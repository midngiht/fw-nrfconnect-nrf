#
# Copyright (c) 2018 Nordic Semiconductor
#
# SPDX-License-Identifier: LicenseRef-BSD-5-Clause-Nordic
#

zephyr_library()
zephyr_library_sources_ifdef(CONFIG_NFC_NDEF_MSG nfc_ndef_msg.c)
zephyr_library_sources_ifdef(CONFIG_NFC_NDEF_RECORD nfc_ndef_record.c)
zephyr_library_sources_ifdef(CONFIG_NFC_NDEF_LE_OOB_REC le_oob_rec.c)
zephyr_library_sources_ifdef(CONFIG_NFC_NDEF_TEXT_RECORD nfc_text_rec.c)
zephyr_library_sources_ifdef(CONFIG_NFC_NDEF_URI_MSG nfc_uri_msg.c)
zephyr_library_sources_ifdef(CONFIG_NFC_NDEF_URI_REC nfc_uri_rec.c)
zephyr_library_sources_ifdef(CONFIG_NFC_NDEF_PARSER msg_parser.c)
zephyr_library_sources_ifdef(CONFIG_NFC_NDEF_PARSER msg_parser_local.c)
zephyr_library_sources_ifdef(CONFIG_NFC_NDEF_PAYLOAD_TYPE_COMMON payload_type_common.c)
zephyr_library_sources_ifdef(CONFIG_NFC_NDEF_PARSER record_parser.c)
zephyr_library_sources_ifdef(CONFIG_NFC_NDEF_TNEP_RECORD tnep_rec.c)
