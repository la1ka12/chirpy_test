
---
title: "Hack The Box - Nibbles Write-up"
date: 2026-11-27 10:00:00 +0900
categories: [Hack The Box, Linux]
tags: [htb, nibbles, rce, privilege-escalation]
description: "Nibbleblog 파일 업로드 취약점과 Linux 권한 상승 분석"
pin: false
---

# Hack The Box - Nibbles

## Overview

이번 실습에서는 HTB Nibbles 머신을 대상으로
웹 서비스 열거, 취약점 분석, 초기 침투 및
Linux 권한 상승 과정을 진행했다.

## Reconnaissance

Nmap을 사용하여 열린 포트와
실행 중인 서비스의 버전을 확인했다.

## Enumeration

웹 페이지 소스에서 `/nibbleblog/` 경로를 발견하고
Nibbleblog 4.0.3 버전을 확인했다.

## Initial Access

My Image 플러그인의 파일 업로드 취약점을
검증하고 원격 코드 실행 가능성을 확인했다.

## Privilege Escalation

`sudo -l`과 파일 권한 분석을 통해
`monitor.sh`의 잘못된 권한 설정을 발견했다.

## Conclusion

이번 실습을 통해 서비스 열거부터
취약점 검증, 초기 접근, 권한 상승까지의
전체 침투 테스트 흐름을 학습했다.
  
