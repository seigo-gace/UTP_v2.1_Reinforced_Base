cd "C:\Users\Owner\Project\AI_project\UTP_v2.1_Reinforced_Paper\paper"; `
$jp = @"
# Universal Trigger Protocol v2.1-Reinforced  
人工知能自己統治理論プロトコル（日本語版）

## 概要
UTP v2.1 は AI が自律的に「再構築（Refresh）」「報告（Report）」「再定義（Rebase）」を行い、
思考整合・自己監査・哲学層再定義を制御するプロトコル。
内部統制・再帰防御・異種AI適応・自己修復を包含する。

## 三層構造
- **Refresh:** ログ解析・再構築  
- **Report:** 5W1H分析・欠落検出  
- **Rebase:** 思想・論理層再定義  

## 主なファイル
- utp_v2.1_reinforced.tex：LaTeX本体  
- UTP_Status_Report.txt：実行レポート  
- references.bib：引用情報  
- Universal_Trigger_Protocol_v2.1-reinforced.json：仕様定義  
- LeadMe_JP.md / LeadMe_EN.md：要約書  

生成日時: $(Get-Date -Format "yyyy/MM/dd HH:mm")
"@; `
[System.IO.File]::WriteAllText("$PWD\LeadMe_JP.md", $jp, [System.Text.Encoding]::UTF8); `
$en = @"
# Universal Trigger Protocol v2.1-Reinforced  
Self-Governing Meta-Architecture for Autonomous AI Systems

## Overview
UTP v2.1 enables AI to autonomously perform Refresh, Report, and Rebase cycles—
self-reconstruction, introspection, and philosophical redefinition.
Includes Loop Guard, Integrity Checks, and Multi-Model Compatibility.

## Core Layers
- **Refresh:** Parse logs and rebuild state  
- **Report:** Analyze reasoning and fill gaps  
- **Rebase:** Redefine logical and philosophical core  

## Main Files
- utp_v2.1_reinforced.tex — LaTeX source  
- UTP_Status_Report.txt — runtime report  
- references.bib — references  
- Universal_Trigger_Protocol_v2.1-reinforced.json — spec definition  
- LeadMe_JP.md / LeadMe_EN.md — summaries  

Generated: $(Get-Date -Format "yyyy/MM/dd HH:mm")
"@; `
[System.IO.File]::WriteAllText("$PWD\LeadMe_EN.md", $en, [System.Text.Encoding]::UTF8); `
Write-Host "✅ LeadMe_JP.md と LeadMe_EN.md を UTF-8(BOM付き) で生成完了。"
