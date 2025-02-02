# This image is used to speed up build process for official netdata images.
#
# Copyright: 2019 and later Netdata Incorporated
# SPDX-License-Identifier: GPL-3.0-or-later
#
# Author : Paul Emm. Katsoulakis <paul@netdata.rocks>
# Author : Austin S. Hemmelgarn <austiN@netdata.cloud>

# This image is used to speed up build process for official netdata images.

FROM alpine:3.15 as builder

# Install some prerequisites
RUN apk --no-cache add apcupsd \
                       curl \
                       fping \
                       iproute2 \
                       jq \
                       json-c \
                       libgcrypt \
                       libmnl \
                       libuuid \
                       libuv \
                       libvirt-daemon \
                       lm-sensors \
                       lz4 \
                       lz4-libs \
                       mongo-c-driver \
                       msmtp \
                       netcat-openbsd \
                       nodejs \
                       openssl \
                       postgresql-client \
                       protobuf \
                       py3-pip \
                       python3 \
                       shadow \
                       snappy \
                       util-linux \
                       zlib

# Add nut dependency from alpine-edge
RUN apk --no-cache add nut --repository http://dl-cdn.alpinelinux.org/alpine/edge/testing --repository http://dl-cdn.alpinelinux.org/alpine/edge/main
