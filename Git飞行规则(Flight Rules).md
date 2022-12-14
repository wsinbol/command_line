# Gité£è¡è§å(Flight Rules)

ð
*[English](README.md) â [EspaÃ±ol](README_es.md)  â  [Ð ÑÑÑÐºÐ¸Ð¹](README_ru.md) â [ç®ä½ä¸­æ](README_zh-CN.md)â [íêµ­ì´](README_kr.md)  â  [Tiáº¿ng Viá»t](README_vi.md) â [FranÃ§ais](README_fr.md) â [æ¥æ¬èª](README_ja.md)*

#### åè¨

- è±æåç[README](https://github.com/k88hudson/git-flight-rules/blob/master/README.md)
- ç¿»è¯å¯è½å­å¨éè¯¯æä¸æ åçå°æ¹ï¼æ¬¢è¿å¤§å®¶ææ­£åä¿®æ¹ï¼è°¢è°¢ï¼

#### ä»ä¹æ¯"é£è¡è§å"?

è¿æ¯ä¸ç¯ç»å®èªåï¼è¿éå°±æ¯æä½¿ç¨Gitçç¨åºåä»¬ï¼çæåï¼ç¨æ¥æå¯¼é®é¢åºç°åçåºå¯¹ä¹æ³ã

>  *é£è¡è§å(Flight Rules)* æ¯è®°å½å¨æåä¸çæ¥ä¹ä¸æçä¸ç³»åç¥è¯ï¼è®°å½äºæä¸ªäºæåççåå ï¼ä»¥åææ ·ä¸æ­¥ä¸æ­¥çè¿è¡å¤çãæ¬è´¨ä¸, å®ä»¬æ¯ç¹å®åºæ¯çéå¸¸è¯¦ç»çæ åå¤çæµç¨ã [...]

> èª20ä¸çºª60å¹´ä»£åä»¥æ¥ï¼NASAä¸ç´å¨ææ(capturing)æä»¬çå¤±è¯¯ï¼ç¾é¾åè§£å³æ¹æ¡, å½æ¶æ°´ææ¶ä»£(Mercury-era)çå°é¢å°ç»é¦åå¼å§å°âç»éªæè®­âæ¶éå°ä¸ä¸ªçº²è¦(compendium)ä¸­ï¼è¯¥çº²ç°å¨å·²ç»æä¸åä¸ªé®é¢ææ¯ï¼ä»åå¨æºæéå°ç ´æçè±å£ææå°è®¡ç®æºæéï¼ä»¥åå®ä»¬å¯¹åºçè§£å³æ¹æ¡ã

&mdash; Chris Hadfield, *ä¸ä¸ªå®èªåççæ´»æå(An Astronaut's Guide to Life)*ã

#### è¿ç¯æç« ççº¦å®

ä¸ºäºæ¸æ¥çè¡¨è¿°ï¼è¿ç¯ææ¡£éçææä¾å­ä½¿ç¨äºèªå®ä¹çbash æç¤ºï¼ä»¥ä¾¿æç¤ºå½ååæ¯åæ¯å¦ææå­çåå(changes)ãåæ¯åç¨å°æ¬å·æ¬èµ·æ¥ï¼åæ¯ååé¢è·ç`*`è¡¨ç¤ºæå­çåå(changes)ã

[![Join the chat at https://gitter.im/k88hudson/git-flight-rules](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/k88hudson/git-flight-rules?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

  - [ç¼è¾æäº¤(editting commits)](#%E7%BC%96%E8%BE%91%E6%8F%90%E4%BA%A4editting-commits)
    - [æåææäº¤äºä»ä¹?](#%E6%88%91%E5%88%9A%E6%89%8D%E6%8F%90%E4%BA%A4%E4%BA%86%E4%BB%80%E4%B9%88)
    - [æçæäº¤ä¿¡æ¯(commit message)åéäº](#%E6%88%91%E7%9A%84%E6%8F%90%E4%BA%A4%E4%BF%A1%E6%81%AFcom mit-message%E5%86%99%E9%94%99%E4%BA%86)
    - [ææäº¤(commit)éçç¨æ·ååé®ç®±ä¸å¯¹](#%E6%88%91%E6%8F%90%E4%BA%A4commit%E9%87%8C%E7%9A%84%E7%94%A8%E6%88%B7%E5%90%8D%E5%92%8C%E9%82%AE%E7%AE%B1%E4%B8%8D%E5%AF%B9)
    - [ææ³ä»ä¸ä¸ªæäº¤(commit)éç§»é¤ä¸ä¸ªæä»¶](#%E6%88%91%E6%83%B3%E4%BB%8E%E4%B8%80%E4%B8%AA%E6%8F%90%E4%BA%A4commit%E9%87%8C%E7%A7%BB%E9%99%A4%E4%B8%80%E4%B8%AA%E6%96%87%E4%BB%B6)
    - [ææ³å é¤æççæåä¸æ¬¡æäº¤(commit)](#%E6%88%91%E6%83%B3%E5%88%A0%E9%99%A4%E6%88%91%E7%9A%84%E7%9A%84%E6%9C%80%E5%90%8E%E4%B8%80%E6%AC%A1%E6%8F%90%E4%BA%A4commit)
    - [å é¤ä»»ææäº¤(commit)](#%E5%88%A0%E9%99%A4%E4%BB%BB%E6%84%8F%E6%8F%90%E4%BA%A4commit)
    - [æå°è¯æ¨ä¸ä¸ªä¿®æ­£åçæäº¤(amended commit)å°è¿ç¨ï¼ä½æ¯æ¥éï¼](#%E6%88%91%E5%B0%9D%E8%AF%95%E6%8E%A8%E4%B8%80%E4%B8%AA%E4%BF%AE%E6%AD%A3%E5%90%8E%E7%9A%84%E6%8F%90%E4%BA%A4amended-commit%E5%88%B0%E8%BF%9C%E7%A8%8B%E4%BD%86%E6%98%AF%E6%8A%A5%E9%94%99)
    - [ææå¤çåäºä¸æ¬¡ç¡¬éç½®(hard reset)ï¼ææ³æ¾åæçåå®¹](#%E6%88%91%E6%84%8F%E5%A4%96%E7%9A%84%E5%81%9A%E4%BA%86%E4%B8%80%E6%AC%A1%E7%A1%AC%E9%87%8D%E7%BD%AEhard-reset%E6%88%91%E6%83%B3%E6%89%BE%E5%9B%9E%E6%88%91%E7%9A%84%E5%86%85%E5%AE%B9)
  - [æå­(Staging)](#%E6%9A%82%E5%AD%98staging)
    - [æéè¦ææå­çåå®¹æ·»å å°ä¸ä¸æ¬¡çæäº¤(commit)](#%E6%88%91%E9%9C%80%E8%A6%81%E6%8A%8A%E6%9A%82%E5%AD%98%E7%9A%84%E5%86%85%E5%AE%B9%E6%B7%BB%E5%8A%A0%E5%88%B0%E4%B8%8A%E4%B8%80%E6%AC%A1%E7%9A%84%E6%8F%90%E4%BA%A4commit)
    - [ææ³è¦æå­ä¸ä¸ªæ°æä»¶çä¸é¨åï¼èä¸æ¯è¿ä¸ªæä»¶çå¨é¨](#%E6%88%91%E6%83%B3%E8%A6%81%E6%9A%82%E5%AD%98%E4%B8%80%E4%B8%AA%E6%96%B0%E6%96%87%E4%BB%B6%E7%9A%84%E4%B8%80%E9%83%A8%E5%88%86%E8%80%8C%E4%B8%8D%E6%98%AF%E8%BF%99%E4%B8%AA%E6%96%87%E4%BB%B6%E7%9A%84%E5%85%A8%E9%83%A8)
    - [ææ³æå¨ä¸ä¸ªæä»¶éçåå(changes)å å°ä¸¤ä¸ªæäº¤(commit)é](#%E6%88%91%E6%83%B3%E6%8A%8A%E5%9C%A8%E4%B8%80%E4%B8%AA%E6%96%87%E4%BB%B6%E9%87%8C%E7%9A%84%E5%8F%98%E5%8C%96changes%E5%8A%A0%E5%88%B0%E4%B8%A4%E4%B8%AA%E6%8F%90%E4%BA%A4commit%E9%87%8C)
    - [ææ³ææå­çåå®¹åææªæå­ï¼ææªæå­çåå®¹æå­èµ·æ¥](#%E6%88%91%E6%83%B3%E6%8A%8A%E6%9A%82%E5%AD%98%E7%9A%84%E5%86%85%E5%AE%B9%E5%8F%98%E6%88%90%E6%9C%AA%E6%9A%82%E5%AD%98%E6%8A%8A%E6%9C%AA%E6%9A%82%E5%AD%98%E7%9A%84%E5%86%85%E5%AE%B9%E6%9A%82%E5%AD%98%E8%B5%B7%E6%9D%A5)
  - [æªæå­(Unstaged)çåå®¹](#%E6%9C%AA%E6%9A%82%E5%AD%98unstaged%E7%9A%84%E5%86%85%E5%AE%B9)
    - [ææ³ææªæå­çåå®¹ç§»å¨å°ä¸ä¸ªæ°åæ¯](#%E6%88%91%E6%83%B3%E6%8A%8A%E6%9C%AA%E6%9A%82%E5%AD%98%E7%9A%84%E5%86%85%E5%AE%B9%E7%A7%BB%E5%8A%A8%E5%88%B0%E4%B8%80%E4%B8%AA%E6%96%B0%E5%88%86%E6%94%AF)
    - [ææ³ææªæå­çåå®¹ç§»å¨å°å¦ä¸ä¸ªå·²å­å¨çåæ¯](#%E6%88%91%E6%83%B3%E6%8A%8A%E6%9C%AA%E6%9A%82%E5%AD%98%E7%9A%84%E5%86%85%E5%AE%B9%E7%A7%BB%E5%8A%A8%E5%88%B0%E5%8F%A6%E4%B8%80%E4%B8%AA%E5%B7%B2%E5%AD%98%E5%9C%A8%E7%9A%84%E5%88%86%E6%94%AF)
    - [ææ³ä¸¢å¼æ¬å°æªæäº¤çåå(uncommitted changes)](#%E6%88%91%E6%83%B3%E4%B8%A2%E5%BC%83%E6%9C%AC%E5%9C%B0%E6%9C%AA%E6%8F%90%E4%BA%A4%E7%9A%84%E5%8F%98%E5%8C%96uncommitted-changes)
    - [ææ³ä¸¢å¼æäºæªæå­çåå®¹](#%E6%88%91%E6%83%B3%E4%B8%A2%E5%BC%83%E6%9F%90%E4%BA%9B%E6%9C%AA%E6%9A%82%E5%AD%98%E7%9A%84%E5%86%85%E5%AE%B9)
  - [åæ¯(Branches)](#%E5%88%86%E6%94%AFbranches)
    - [æä»éè¯¯çåæ¯æåäºåå®¹ï¼ææåå®¹æåå°äºéè¯¯çåæ¯](#%E6%88%91%E4%BB%8E%E9%94%99%E8%AF%AF%E7%9A%84%E5%88%86%E6%94%AF%E6%8B%89%E5%8F%96%E4%BA%86%E5%86%85%E5%AE%B9%E6%88%96%E6%8A%8A%E5%86%85%E5%AE%B9%E6%8B%89%E5%8F%96%E5%88%B0%E4%BA%86%E9%94%99%E8%AF%AF%E7%9A%84%E5%88%86%E6%94%AF)
    - [ææ³æææ¬å°çæäº¤(commit)ï¼ä»¥ä¾¿æçåæ¯ä¸è¿ç¨çä¿æä¸è´](#%E6%88%91%E6%83%B3%E6%89%94%E6%8E%89%E6%9C%AC%E5%9C%B0%E7%9A%84%E6%8F%90%E4%BA%A4commit%E4%BB%A5%E4%BE%BF%E6%88%91%E7%9A%84%E5%88%86%E6%94%AF%E4%B8%8E%E8%BF%9C%E7%A8%8B%E7%9A%84%E4%BF%9D%E6%8C%81%E4%B8%80%E8%87%B4)
    - [æéè¦æäº¤å°ä¸ä¸ªæ°åæ¯ï¼ä½éè¯¯çæäº¤å°äºmain](#%E6%88%91%E9%9C%80%E8%A6%81%E6%8F%90%E4%BA%A4%E5%88%B0%E4%B8%80%E4%B8%AA%E6%96%B0%E5%88%86%E6%94%AF%E4%BD%86%E9%94%99%E8%AF%AF%E7%9A%84%E6%8F%90%E4%BA%A4%E5%88%B0%E4%BA%86main)
    - [ææ³ä¿çæ¥èªå¦å¤ä¸ä¸ªref-ishçæ´ä¸ªæä»¶](#%E6%88%91%E6%83%B3%E4%BF%9D%E7%95%99%E6%9D%A5%E8%87%AA%E5%8F%A6%E5%A4%96%E4%B8%80%E4%B8%AAref-ish%E7%9A%84%E6%95%B4%E4%B8%AA%E6%96%87%E4%BB%B6)
    - [ææå ä¸ªæäº¤(commit)æäº¤å°äºåä¸ä¸ªåæ¯ï¼èè¿äºæäº¤åºè¯¥åå¸å¨ä¸åçåæ¯é](#%E6%88%91%E6%8A%8A%E5%87%A0%E4%B8%AA%E6%8F%90%E4%BA%A4commit%E6%8F%90%E4%BA%A4%E5%88%B0%E4%BA%86%E5%90%8C%E4%B8%80%E4%B8%AA%E5%88%86%E6%94%AF%E8%80%8C%E8%BF%99%E4%BA%9B%E6%8F%90%E4%BA%A4%E5%BA%94%E8%AF%A5%E5%88%86%E5%B8%83%E5%9C%A8%E4%B8%8D%E5%90%8C%E7%9A%84%E5%88%86%E6%94%AF%E9%87%8C)
    - [ææ³å é¤ä¸æ¸¸(upstream)åæ¯è¢«å é¤äºçæ¬å°åæ¯](#%E6%88%91%E6%83%B3%E5%88%A0%E9%99%A4%E4%B8%8A%E6%B8%B8upstream%E5%88%86%E6%94%AF%E8%A2%AB%E5%88%A0%E9%99%A4%E4%BA%86%E7%9A%84%E6%9C%AC%E5%9C%B0%E5%88%86%E6%94%AF)
    - [æä¸å°å¿å é¤äºæçåæ¯](#%E6%88%91%E4%B8%8D%E5%B0%8F%E5%BF%83%E5%88%A0%E9%99%A4%E4%BA%86%E6%88%91%E7%9A%84%E5%88%86%E6%94%AF)
    - [ææ³å é¤ä¸ä¸ªåæ¯](#%E6%88%91%E6%83%B3%E5%88%A0%E9%99%A4%E4%B8%80%E4%B8%AA%E5%88%86%E6%94%AF)
    - [ææ³ä»å«äººæ­£å¨å·¥ä½çè¿ç¨åæ¯ç­¾åº(checkout)ä¸ä¸ªåæ¯](#%E6%88%91%E6%83%B3%E4%BB%8E%E5%88%AB%E4%BA%BA%E6%AD%A3%E5%9C%A8%E5%B7%A5%E4%BD%9C%E7%9A%84%E8%BF%9C%E7%A8%8B%E5%88%86%E6%94%AF%E7%AD%BE%E5%87%BAcheckout%E4%B8%80%E4%B8%AA%E5%88%86%E6%94%AF)
  - [Rebasing ååå¹¶(Merging)](#rebasing-%E5%92%8C%E5%90%88%E5%B9%B6merging)
    - [ææ³æ¤érebase/merge](#%E6%88%91%E6%83%B3%E6%92%A4%E9%94%80rebasemerge)
    - [æå·²ç»rebaseè¿, ä½æ¯æä¸æ³å¼ºæ¨(force push)](#%E6%88%91%E5%B7%B2%E7%BB%8Frebase%E8%BF%87-%E4%BD%86%E6%98%AF%E6%88%91%E4%B8%8D%E6%83%B3%E5%BC%BA%E6%8E%A8force-push)
    - [æéè¦ç»å(combine)å ä¸ªæäº¤(commit)](#%E6%88%91%E9%9C%80%E8%A6%81%E7%BB%84%E5%90%88combine%E5%87%A0%E4%B8%AA%E6%8F%90%E4%BA%A4commit)
      - [å®å¨åå¹¶(merging)ç­ç¥](#%E5%AE%89%E5%85%A8%E5%90%88%E5%B9%B6merging%E7%AD%96%E7%95%A5)
      - [æéè¦å°ä¸ä¸ªåæ¯åå¹¶æä¸ä¸ªæäº¤(commit)](#%E6%88%91%E9%9C%80%E8%A6%81%E5%B0%86%E4%B8%80%E4%B8%AA%E5%88%86%E6%94%AF%E5%90%88%E5%B9%B6%E6%88%90%E4%B8%80%E4%B8%AA%E6%8F%90%E4%BA%A4commit)
      - [æåªæ³ç»å(combine)æªæ¨çæäº¤(unpushed commit)](#%E6%88%91%E5%8F%AA%E6%83%B3%E7%BB%84%E5%90%88combine%E6%9C%AA%E6%8E%A8%E7%9A%84%E6%8F%90%E4%BA%A4unpushed-commit)
    - [æ£æ¥æ¯å¦åæ¯ä¸çæææäº¤(commit)é½åå¹¶(merge)è¿äº](#%E6%A3%80%E6%9F%A5%E6%98%AF%E5%90%A6%E5%88%86%E6%94%AF%E4%B8%8A%E7%9A%84%E6%89%80%E6%9C%89%E6%8F%90%E4%BA%A4commit%E9%83%BD%E5%90%88%E5%B9%B6merge%E8%BF%87%E4%BA%86)
    - [äº¤äºå¼rebase(interactive rebase)å¯è½åºç°çé®é¢](#%E4%BA%A4%E4%BA%92%E5%BC%8Frebaseinteractive-rebase%E5%8F%AF%E8%83%BD%E5%87%BA%E7%8E%B0%E7%9A%84%E9%97%AE%E9%A2%98)
      - [è¿ä¸ªrebase ç¼è¾å±å¹åºç°'noop'](#%E8%BF%99%E4%B8%AArebase-%E7%BC%96%E8%BE%91%E5%B1%8F%E5%B9%95%E5%87%BA%E7%8E%B0noop)
      - [æå²çªçæåµ](#%E6%9C%89%E5%86%B2%E7%AA%81%E7%9A%84%E6%83%85%E5%86%B5)
  - [Stash](#stash)
    - [æå­æææ¹å¨](#%E6%9A%82%E5%AD%98%E6%89%80%E6%9C%89%E6%94%B9%E5%8A%A8)
    - [æå­æå®æä»¶](#%E6%9A%82%E5%AD%98%E6%8C%87%E5%AE%9A%E6%96%87%E4%BB%B6)
    - [æå­æ¶è®°å½æ¶æ¯](#%E6%9A%82%E5%AD%98%E6%97%B6%E8%AE%B0%E5%BD%95%E6%B6%88%E6%81%AF)
    - [ä½¿ç¨æä¸ªæå®æå­](#%E4%BD%BF%E7%94%A8%E6%9F%90%E4%B8%AA%E6%8C%87%E5%AE%9A%E6%9A%82%E5%AD%98)
    - [æå­æ¶ä¿çæªæå­çåå®¹](#%E6%9A%82%E5%AD%98%E6%97%B6%E4%BF%9D%E7%95%99%E6%9C%AA%E6%9A%82%E5%AD%98%E7%9A%84%E5%86%85%E5%AE%B9)
  - [æé¡¹(Miscellaneous Objects)](#%E6%9D%82%E9%A1%B9miscellaneous-objects)
    - [åéææå­æ¨¡å](#%E5%85%8B%E9%9A%86%E6%89%80%E6%9C%89%E5%AD%90%E6%A8%A1%E5%9D%97)
    - [å é¤æ ç­¾(tag)](#%E5%88%A0%E9%99%A4%E6%A0%87%E7%AD%BEtag)
    - [æ¢å¤å·²å é¤æ ç­¾(tag)](#%E6%81%A2%E5%A4%8D%E5%B7%B2%E5%88%A0%E9%99%A4%E6%A0%87%E7%AD%BEtag)
    - [å·²å é¤è¡¥ä¸(patch)](#%E5%B7%B2%E5%88%A0%E9%99%A4%E8%A1%A5%E4%B8%81patch)
  - [è·è¸ªæä»¶(Tracking Files)](#%E8%B7%9F%E8%B8%AA%E6%96%87%E4%BB%B6tracking-files)
    - [æåªæ³æ¹åä¸ä¸ªæä»¶åå­çå¤§å°åï¼èä¸ä¿®æ¹åå®¹](#%E6%88%91%E5%8F%AA%E6%83%B3%E6%94%B9%E5%8F%98%E4%B8%80%E4%B8%AA%E6%96%87%E4%BB%B6%E5%90%8D%E5%AD%97%E7%9A%84%E5%A4%A7%E5%B0%8F%E5%86%99%E8%80%8C%E4%B8%8D%E4%BF%AE%E6%94%B9%E5%86%85%E5%AE%B9)
    - [ææ³ä»Gitå é¤ä¸ä¸ªæä»¶ï¼ä½ä¿çè¯¥æä»¶](#%E6%88%91%E6%83%B3%E4%BB%8Egit%E5%88%A0%E9%99%A4%E4%B8%80%E4%B8%AA%E6%96%87%E4%BB%B6%E4%BD%86%E4%BF%9D%E7%95%99%E8%AF%A5%E6%96%87%E4%BB%B6)
  - [éç½®(Configuration)](#%E9%85%8D%E7%BD%AEconfiguration)
    - [ææ³ç»ä¸äºGitå½ä»¤æ·»å å«å(alias)](#%E6%88%91%E6%83%B3%E7%BB%99%E4%B8%80%E4%BA%9Bgit%E5%91%BD%E4%BB%A4%E6%B7%BB%E5%8A%A0%E5%88%AB%E5%90%8Dalias)
    - [ææ³ç¼å­ä¸ä¸ªä»åº(repository)çç¨æ·ååå¯ç ](#%E6%88%91%E6%83%B3%E7%BC%93%E5%AD%98%E4%B8%80%E4%B8%AA%E4%BB%93%E5%BA%93repository%E7%9A%84%E7%94%A8%E6%88%B7%E5%90%8D%E5%92%8C%E5%AF%86%E7%A0%81)
  - [æä¸ç¥éæåéäºäºä»ä¹](#%E6%88%91%E4%B8%8D%E7%9F%A5%E9%81%93%E6%88%91%E5%81%9A%E9%94%99%E4%BA%86%E4%BA%9B%E4%BB%80%E4%B9%88)
- [å¶å®èµæº(Other Resources)](#%E5%85%B6%E5%AE%83%E8%B5%84%E6%BA%90other-resources)
  - [ä¹¦(Books)](#%E4%B9%A6books)
  - [æç¨(Tutorials)](#%E6%95%99%E7%A8%8Btutorials)
  - [èæ¬åå·¥å·(Scripts and Tools)](#%E8%84%9A%E6%9C%AC%E5%92%8C%E5%B7%A5%E5%85%B7scripts-and-tools)
  - [GUIå®¢æ·ç«¯(GUI Clients)](#gui%E5%AE%A2%E6%88%B7%E7%AB%AFgui-clients)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## ç¼è¾æäº¤(editting commits)

<a name="diff-last"></a>
### æåææäº¤äºä»ä¹?

å¦æä½ ç¨ `git commit -a` æäº¤äºä¸æ¬¡åå(changes)ï¼èä½ åä¸ç¡®å®å°åºè¿æ¬¡æäº¤äºåªäºåå®¹ã ä½ å°±å¯ä»¥ç¨ä¸é¢çå½ä»¤æ¾ç¤ºå½å`HEAD`ä¸çæè¿ä¸æ¬¡çæäº¤(commit):

```sh
(main)$ git show
```

æè

```sh
$ git log -n1 -p
```

<a name="#i-wrote-the-wrong-thing-in-a-commit-message"></a>
### æçæäº¤ä¿¡æ¯(commit message)åéäº

å¦æä½ çæäº¤ä¿¡æ¯(commit message)åéäºä¸è¿æ¬¡æäº¤(commit)è¿æ²¡ææ¨(push), ä½ å¯ä»¥éè¿ä¸é¢çæ¹æ³æ¥ä¿®æ¹æäº¤ä¿¡æ¯(commit message):

```sh
$ git commit --amend --only
```
è¿ä¼æå¼ä½ çé»è®¤ç¼è¾å¨, å¨è¿éä½ å¯ä»¥ç¼è¾ä¿¡æ¯. å¦ä¸æ¹é¢, ä½ ä¹å¯ä»¥ç¨ä¸æ¡å½ä»¤ä¸æ¬¡å®æ:

```sh
$ git commit --amend --only -m 'xxxxxxx'
```

å¦æä½ å·²ç»æ¨(push)äºè¿æ¬¡æäº¤(commit), ä½ å¯ä»¥ä¿®æ¹è¿æ¬¡æäº¤(commit)ç¶åå¼ºæ¨(force push), ä½æ¯ä¸æ¨èè¿ä¹åã

<a name="commit-wrong-author"></a>
### ææäº¤(commit)éçç¨æ·ååé®ç®±ä¸å¯¹

å¦æè¿åªæ¯åä¸ªæäº¤(commit)ï¼ä¿®æ¹å®ï¼

```sh
$ git commit --amend --author "New Authorname <authoremail@mydomain.com>"
```

å¦æä½ éè¦ä¿®æ¹ææåå², åè 'git filter-branch'çæåé¡µ.

<a href="#i-want-to-remove-a-file-from-a-commit"></a>
### ææ³ä»ä¸ä¸ªæäº¤(commit)éç§»é¤ä¸ä¸ªæä»¶

éè¿ä¸é¢çæ¹æ³ï¼ä»ä¸ä¸ªæäº¤(commit)éç§»é¤ä¸ä¸ªæä»¶:

```sh
$ git checkout HEAD^ myfile
$ git add -A
$ git commit --amend
```

è¿å°éå¸¸æç¨ï¼å½ä½ æä¸ä¸ªå¼æ¾çè¡¥ä¸(open patch)ï¼ä½ å¾ä¸é¢æäº¤äºä¸ä¸ªä¸å¿è¦çæä»¶ï¼ä½ éè¦å¼ºæ¨(force push)å»æ´æ°è¿ä¸ªè¿ç¨è¡¥ä¸ã

<a name="delete-pushed-commit"></a>
### ææ³å é¤æççæåä¸æ¬¡æäº¤(commit)

å¦æä½ éè¦å é¤æ¨äºçæäº¤(pushed commits)ï¼ä½ å¯ä»¥ä½¿ç¨ä¸é¢çæ¹æ³ãå¯æ¯ï¼è¿ä¼ä¸å¯éçæ¹åä½ çåå²ï¼ä¹ä¼æä¹±é£äºå·²ç»ä»è¯¥ä»åºæå(pulled)äºçäººçåå²ãç®èè¨ä¹ï¼å¦æä½ ä¸æ¯å¾ç¡®å®ï¼åä¸ä¸è¦è¿ä¹åã

```sh
$ git reset HEAD^ --hard
$ git push -f [remote] [branch]
```

å¦æä½ è¿æ²¡ææ¨å°è¿ç¨, æGitéç½®(reset)å°ä½ æåä¸æ¬¡æäº¤åçç¶æå°±å¯ä»¥äº(åæ¶ä¿å­æå­çåå):

```
(my-branch*)$ git reset --soft HEAD@{1}

```

è¿åªè½å¨æ²¡ææ¨éä¹åæç¨. å¦æä½ å·²ç»æ¨äº, å¯ä¸å®å¨è½åçæ¯ `git revert SHAofBadCommit`ï¼ é£ä¼åå»ºä¸ä¸ªæ°çæäº¤(commit)ç¨äºæ¤æ¶åä¸ä¸ªæäº¤çææåå(changes)ï¼ æè, å¦æä½ æ¨çè¿ä¸ªåæ¯æ¯rebase-safeç (ä¾å¦ï¼ å¶å®å¼åèä¸ä¼ä»è¿ä¸ªåæ¯æ), åªéè¦ä½¿ç¨ `git push -f`ï¼ æ´å¤, è¯·åè [the above section](#deleteremove-last-pushed-commit)ã

<a name="delete-any-commit"></a>
### å é¤ä»»ææäº¤(commit)

åæ ·çè­¦åï¼ä¸å°ä¸ä¸å¾å·²çæ¶åä¸è¦è¿ä¹å.

```sh
$ git rebase --onto SHA1_OF_BAD_COMMIT^ SHA1_OF_BAD_COMMIT
$ git push -f [remote] [branch]
```

æèåä¸ä¸ª [äº¤äºå¼rebase](#interactive-rebase) å é¤é£äºä½ æ³è¦å é¤çæäº¤(commit)éæå¯¹åºçè¡ã

<a name="#force-push"></a>
### æå°è¯æ¨ä¸ä¸ªä¿®æ­£åçæäº¤(amended commit)å°è¿ç¨ï¼ä½æ¯æ¥éï¼

```sh
To https://github.com/yourusername/repo.git
! [rejected]        mybranch -> mybranch (non-fast-forward)
error: failed to push some refs to 'https://github.com/tanay1337/webmaker.org.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```

æ³¨æ, rebasing(è§ä¸é¢)åä¿®æ­£(amending)ä¼ç¨ä¸ä¸ª**æ°çæäº¤(commit)ä»£æ¿æ§ç**, æä»¥å¦æä¹åä½ å·²ç»å¾è¿ç¨ä»åºä¸æ¨è¿ä¸æ¬¡ä¿®æ­£åçæäº¤(commit)ï¼é£ä½ ç°å¨å°±å¿é¡»å¼ºæ¨(force push) (`-f`)ã æ³¨æ &ndash; *æ»æ¯* ç¡®ä¿ä½ ææä¸ä¸ªåæ¯!

```sh
(my-branch)$ git push origin mybranch -f
```

ä¸è¬æ¥è¯´, **è¦é¿åå¼ºæ¨**. æå¥½æ¯åå»ºåæ¨(push)ä¸ä¸ªæ°çæäº¤(commit)ï¼èä¸æ¯å¼ºæ¨ä¸ä¸ªä¿®æ­£åçæäº¤ãåèä¼ä½¿é£äºä¸è¯¥åæ¯æè¯¥åæ¯çå­åæ¯å·¥ä½çå¼åèï¼å¨æºåå²ä¸­äº§çå²çªã

<a href="undo-git-reset-hard"></a>
### ææå¤çåäºä¸æ¬¡ç¡¬éç½®(hard reset)ï¼ææ³æ¾åæçåå®¹

å¦æä½ æå¤çåäº `git reset --hard`, ä½ éå¸¸è½æ¾åä½ çæäº¤(commit), å ä¸ºGitå¯¹æ¯ä»¶äºé½ä¼ææ¥å¿ï¼ä¸é½ä¼ä¿å­å å¤©ã

```sh
(main)$ git reflog
```

ä½ å°ä¼çå°ä¸ä¸ªä½ è¿å»æäº¤(commit)çåè¡¨, åä¸ä¸ªéç½®çæäº¤ã éæ©ä½ æ³è¦åå°çæäº¤(commit)çSHAï¼åéç½®ä¸æ¬¡:

```sh
(main)$ git reset --hard SHA1234
```

è¿æ ·å°±å®æäºã

## æå­(Staging)

<a href="#i-need-to-add-staged-changes-to-the-previous-commit"></a>
### æéè¦ææå­çåå®¹æ·»å å°ä¸ä¸æ¬¡çæäº¤(commit)

```sh
(my-branch*)$ git commit --amend

```

<a name="commit-partial-new-file"></a>
### ææ³è¦æå­ä¸ä¸ªæ°æä»¶çä¸é¨åï¼èä¸æ¯è¿ä¸ªæä»¶çå¨é¨

ä¸è¬æ¥è¯´, å¦æä½ æ³æå­ä¸ä¸ªæä»¶çä¸é¨å, ä½ å¯è¿æ ·å:

```sh
$ git add --patch filename.x
```

`-p` ç®åãè¿ä¼æå¼äº¤äºæ¨¡å¼ï¼ ä½ å°è½å¤ç¨ `s` éé¡¹æ¥åéæäº¤(commit)ï¼ ç¶è, å¦æè¿ä¸ªæä»¶æ¯æ°ç, ä¼æ²¡æè¿ä¸ªéæ©ï¼ æ·»å ä¸ä¸ªæ°æä»¶æ¶, è¿æ ·å:

```sh
$ git add -N filename.x
```

ç¶å, ä½ éè¦ç¨ `e` éé¡¹æ¥æå¨éæ©éè¦æ·»å çè¡ï¼æ§è¡ `git diff --cached` å°ä¼æ¾ç¤ºåªäºè¡æå­äºåªäºè¡åªæ¯ä¿å­å¨æ¬å°äºã

<a href="stage-in-two-commits"></a>
### ææ³æå¨ä¸ä¸ªæä»¶éçåå(changes)å å°ä¸¤ä¸ªæäº¤(commit)é

`git add` ä¼ææ´ä¸ªæä»¶å å¥å°ä¸ä¸ªæäº¤. `git add -p` åè®¸äº¤äºå¼çéæ©ä½ æ³è¦æäº¤çé¨å.

<a href="unstaging-edits-and-staging-the-unstaged"></a>
### ææ³ææå­çåå®¹åææªæå­ï¼ææªæå­çåå®¹æå­èµ·æ¥

å¤æ°æåµä¸ï¼ä½ åºè¯¥å°ææçåå®¹åä¸ºæªæå­ï¼ç¶ååéæ©ä½ æ³è¦çåå®¹è¿è¡commitã
ä½åå®ä½ å°±æ¯æ³è¦è¿ä¹åï¼è¿éä½ å¯ä»¥åå»ºä¸ä¸ªä¸´æ¶çcommitæ¥ä¿å­ä½ å·²æå­çåå®¹ï¼ç¶åæå­ä½ çæªæå­çåå®¹å¹¶è¿è¡stashãç¶åresetæåä¸ä¸ªcommitå°åæ¬æå­çåå®¹åä¸ºæªæå­ï¼æåstash popåæ¥ã

```sh
$ git commit -m "WIP"
$ git add .
$ git stash
$ git reset HEAD^
$ git stash pop --index 0
```

æ³¨æ1: è¿éä½¿ç¨`pop`ä»ä»æ¯å ä¸ºæ³å°½å¯è½ä¿æå¹ç­ã
æ³¨æ2: åå¦ä½ ä¸å ä¸`--index`ä½ ä¼ææå­çæä»¶æ è®°ä¸ºä¸ºå­å¨.è¿ä¸ª[é¾æ¥](https://stackoverflow.com/questions/31595873/git-stash-with-staged-files-does-stash-convert-staged-files-to-unstaged?answertab=active#tab-top) è§£éå¾æ¯è¾æ¸æ¥ãï¼ä¸è¿æ¯è±æçï¼å¶å¤§ææ¯è¯´ï¼è¿æ¯ä¸ä¸ªè¾ä¸ºåºå±çé®é¢ï¼stashæ¶ä¼å2ä¸ªcommitï¼å¶ä¸­ä¸ä¸ªä¼è®°å½indexç¶æï¼stagedçæä»¶ç­ä¸è¥¿ï¼å¦ä¸ä¸ªè®°å½worktreeåå¶ä»çä¸äºä¸è¥¿ï¼å¦æä½ ä¸å¨applyæ¶å indexï¼gitä¼æä¸¤ä¸ªä¸èµ·éæ¯ï¼æä»¥stagedéå°±ç©ºäºï¼ã

## æªæå­(Unstaged)çåå®¹

<a href="move-unstaged-edits-to-new-branch"></a>
### ææ³ææªæå­çåå®¹ç§»å¨å°ä¸ä¸ªæ°åæ¯

```sh
$ git checkout -b my-branch
```

<a href="move-unstaged-edits-to-old-branch"></a>
### ææ³ææªæå­çåå®¹ç§»å¨å°å¦ä¸ä¸ªå·²å­å¨çåæ¯

```sh
$ git stash
$ git checkout my-branch
$ git stash pop
```

<a href="i-want-to-discard-my-local-uncommitted-changes"></a>
### ææ³ä¸¢å¼æ¬å°æªæäº¤çåå(uncommitted changes)

å¦æä½ åªæ¯æ³éç½®æº(origin)åä½ æ¬å°(local)ä¹é´çä¸äºæäº¤(commit)ï¼ä½ å¯ä»¥ï¼

```sh
# one commit
(my-branch)$ git reset --hard HEAD^
# two commits
(my-branch)$ git reset --hard HEAD^^
# four commits
(my-branch)$ git reset --hard HEAD~4
# or
(main)$ git checkout -f
```

éç½®æä¸ªç¹æ®çæä»¶, ä½ å¯ä»¥ç¨æä»¶ååä¸ºåæ°:

```sh
$ git reset filename
```

<a href="i-want-to-discard-specific-unstaged-changes"></a>
### ææ³ä¸¢å¼æäºæªæå­çåå®¹

å¦æä½ æ³ä¸¢å¼å·¥ä½æ·è´ä¸­çä¸é¨ååå®¹ï¼èä¸æ¯å¨é¨ã

ç­¾åº(checkout)ä¸éè¦çåå®¹ï¼ä¿çéè¦çã

```sh
$ git checkout -p
# Answer y to all of the snippets you want to drop
```

å¦å¤ä¸ä¸ªæ¹æ³æ¯ä½¿ç¨ `stash`ï¼ Stashææè¦ä¿çä¸çåå®¹, éç½®å·¥ä½æ·è´, éæ°åºç¨ä¿ççé¨åã

```sh
$ git stash -p
# Select all of the snippets you want to save
$ git reset --hard
$ git stash pop
```

æè, stash ä½ ä¸éè¦çé¨å, ç¶åstash dropã

```sh
$ git stash -p
# Select all of the snippets you don't want to save
$ git stash drop
```

## åæ¯(Branches)

<a name="pull-wrong-branch"></a>
### æä»éè¯¯çåæ¯æåäºåå®¹ï¼ææåå®¹æåå°äºéè¯¯çåæ¯

è¿æ¯å¦å¤ä¸ç§ä½¿ç¨ `git reflog` æåµï¼æ¾å°å¨è¿æ¬¡éè¯¯æ(pull) ä¹åHEADçæåã

```sh
(main)$ git reflog
ab7555f HEAD@{0}: pull origin wrong-branch: Fast-forward
c5bc55a HEAD@{1}: checkout: checkout message goes here
```

éç½®åæ¯å°ä½ æéçæäº¤(desired commit):

```sh
$ git reset --hard c5bc55a
```

å®æã

<a href="discard-local-commits"></a>
### ææ³æææ¬å°çæäº¤(commit)ï¼ä»¥ä¾¿æçåæ¯ä¸è¿ç¨çä¿æä¸è´

åç¡®è®¤ä½ æ²¡ææ¨(push)ä½ çåå®¹å°è¿ç¨ã

`git status` ä¼æ¾ç¤ºä½ é¢å(ahead)æº(origin)å¤å°ä¸ªæäº¤:

```sh
(my-branch)$ git status
# On branch my-branch
# Your branch is ahead of 'origin/my-branch' by 2 commits.
#   (use "git push" to publish your local commits)
#
```

ä¸ç§æ¹æ³æ¯:

```sh
(main)$ git reset --hard origin/my-branch
```

<a name="commit-wrong-branch"></a>
### æéè¦æäº¤å°ä¸ä¸ªæ°åæ¯ï¼ä½éè¯¯çæäº¤å°äºmain

å¨mainä¸åå»ºä¸ä¸ªæ°åæ¯ï¼ä¸åæ¢å°æ°åæ¯,ä»å¨mainä¸:

```sh
(main)$ git branch my-branch
```

æmainåæ¯éç½®å°åä¸ä¸ªæäº¤:

```sh
(main)$ git reset --hard HEAD^
```

`HEAD^` æ¯ `HEAD^1` çç®åï¼ä½ å¯ä»¥éè¿æå®è¦è®¾ç½®ç`HEAD`æ¥è¿ä¸æ­¥éç½®ã

æè, å¦æä½ ä¸æ³ä½¿ç¨ `HEAD^`, æ¾å°ä½ æ³éç½®å°çæäº¤(commit)çhash(`git log` è½å¤å®æ)ï¼ ç¶åéç½®å°è¿ä¸ªhashã ä½¿ç¨`git push` åæ­¥åå®¹å°è¿ç¨ã

ä¾å¦, mainåæ¯æ³éç½®å°çæäº¤çhashä¸º`a13b85e`:

```sh
(main)$ git reset --hard a13b85e
HEAD is now at a13b85e
```

ç­¾åº(checkout)åææ°å»ºçåæ¯ç»§ç»­å·¥ä½:

```sh
(main)$ git checkout my-branch
```

<a name="keep-whole-file"></a>
### ææ³ä¿çæ¥èªå¦å¤ä¸ä¸ªref-ishçæ´ä¸ªæä»¶

åè®¾ä½ æ­£å¨åä¸ä¸ªååæ¹æ¡(åæä¸ºworking spike (see note)), ææç¾çåå®¹ï¼æ¯ä¸ªé½å·¥ä½å¾å¾å¥½ãç°å¨, ä½ æäº¤å°äºä¸ä¸ªåæ¯ï¼ä¿å­å·¥ä½åå®¹:

```sh
(solution)$ git add -A && git commit -m "Adding all changes from this spike into one big commit."
```

å½ä½ æ³è¦æå®æ¾å°ä¸ä¸ªåæ¯é (å¯è½æ¯`feature`, æè `develop`), ä½ å³å¿æ¯ä¿ææ´ä¸ªæä»¶çå®æ´ï¼ä½ æ³è¦ä¸ä¸ªå¤§çæäº¤åéææ¯è¾å°ã

åè®¾ä½ æ:

  * åæ¯ `solution`, æ¥æååæ¹æ¡ï¼ é¢å `develop` åæ¯ã
  * åæ¯ `develop`, å¨è¿éä½ åºç¨ååæ¹æ¡çä¸äºåå®¹ã

æå»å¯ä»¥éè¿æåå®¹æ¿å°ä½ çåæ¯éï¼æ¥è§£å³è¿ä¸ªé®é¢:

```sh
(develop)$ git checkout solution -- file1.txt
```

è¿ä¼æè¿ä¸ªæä»¶åå®¹ä»åæ¯ `solution` æ¿å°åæ¯ `develop` éæ¥:

```sh
# On branch develop
# Your branch is up-to-date with 'origin/develop'.
# Changes to be committed:
#  (use "git reset HEAD <file>..." to unstage)
#
#        modified:   file1.txt
```

ç¶å, æ­£å¸¸æäº¤ã

Note: Spike solutions are made to analyze or solve the problem. These solutions are used for estimation and discarded once everyone gets clear visualization of the problem. ~ [Wikipedia](https://en.wikipedia.org/wiki/Extreme_programming_practices).

<a name="cherry-pick"></a>
### ææå ä¸ªæäº¤(commit)æäº¤å°äºåä¸ä¸ªåæ¯ï¼èè¿äºæäº¤åºè¯¥åå¸å¨ä¸åçåæ¯é

åè®¾ä½ æä¸ä¸ª`main`åæ¯ï¼ æ§è¡`git log`, ä½ çå°ä½ åè¿ä¸¤æ¬¡æäº¤:

```sh
(main)$ git log

commit e3851e817c451cc36f2e6f3049db528415e3c114
Author: Alex Lee <alexlee@example.com>
Date:   Tue Jul 22 15:39:27 2014 -0400

    Bug #21 - Added CSRF protection

commit 5ea51731d150f7ddc4a365437931cd8be3bf3131
Author: Alex Lee <alexlee@example.com>
Date:   Tue Jul 22 15:39:12 2014 -0400

    Bug #14 - Fixed spacing on title

commit a13b85e984171c6e2a1729bb061994525f626d14
Author: Aki Rose <akirose@example.com>
Date:   Tue Jul 21 01:12:48 2014 -0400

    First commit
```

è®©æä»¬ç¨æäº¤hash(commit hash)æ è®°bug (`e3851e8` for #21, `5ea5173` for #14).

é¦å, æä»¬æ`main`åæ¯éç½®å°æ­£ç¡®çæäº¤(`a13b85e`):

```sh
(main)$ git reset --hard a13b85e
HEAD is now at a13b85e
```

ç°å¨, æä»¬å¯¹ bug #21 åå»ºä¸ä¸ªæ°çåæ¯:

```sh
(main)$ git checkout -b 21
(21)$
```

æ¥ç, æä»¬ç¨ *cherry-pick* æå¯¹bug #21çæäº¤æ¾å¥å½ååæ¯ã è¿æå³çæä»¬å°åºç¨(apply)è¿ä¸ªæäº¤(commit)ï¼ä»ä»è¿ä¸ä¸ªæäº¤(commit)ï¼ç´æ¥å¨HEADä¸é¢ã

```sh
(21)$ git cherry-pick e3851e8
```

è¿æ¶å, è¿éå¯è½ä¼äº§çå²çªï¼ åè§[äº¤äºå¼ rebasing ç« ](#interactive-rebase) [**å²çªè**](#merge-conflict) è§£å³å²çª.

åèï¼ æä»¬ä¸ºbug #14 åå»ºä¸ä¸ªæ°çåæ¯, ä¹åºäº`main`åæ¯

```sh
(21)$ git checkout main
(main)$ git checkout -b 14
(14)$
```

æå, ä¸º bug #14 æ§è¡ `cherry-pick`:

```sh
(14)$ git cherry-pick 5ea5173
```

<a name="delete-stale-local-branches"></a>
### ææ³å é¤ä¸æ¸¸(upstream)åæ¯è¢«å é¤äºçæ¬å°åæ¯
ä¸æ¦ä½ å¨github ä¸é¢åå¹¶(merge)äºä¸ä¸ªpull request, ä½ å°±å¯ä»¥å é¤ä½ forkéè¢«åå¹¶çåæ¯ã å¦æä½ ä¸åå¤ç»§ç»­å¨è¿ä¸ªåæ¯éå·¥ä½, å é¤è¿ä¸ªåæ¯çæ¬å°æ·è´ä¼æ´å¹²åï¼ä½¿ä½ ä¸ä¼é·å¥å·¥ä½åæ¯åä¸å éæ§åæ¯çæ··ä¹±ä¹ä¸­ã

```sh
$ git fetch -p
```

<a name='restore-a-deleted-branch'></a>
### æä¸å°å¿å é¤äºæçåæ¯

å¦æä½ å®ææ¨éå°è¿ç¨, å¤æ°æåµä¸åºè¯¥æ¯å®å¨çï¼ä½æäºæ¶åè¿æ¯å¯è½å é¤äºè¿æ²¡ææ¨å°è¿ç¨çåæ¯ã è®©æä»¬ååå»ºä¸ä¸ªåæ¯åä¸ä¸ªæ°çæä»¶:

```sh
(main)$ git checkout -b my-branch
(my-branch)$ git branch
(my-branch)$ touch foo.txt
(my-branch)$ ls
README.md foo.txt
```

æ·»å æä»¶å¹¶åä¸æ¬¡æäº¤

```sh
(my-branch)$ git add .
(my-branch)$ git commit -m 'foo.txt added'
(my-branch)$ foo.txt added
 1 files changed, 1 insertions(+)
 create mode 100644 foo.txt
(my-branch)$ git log

commit 4e3cd85a670ced7cc17a2b5d8d3d809ac88d5012
Author: siemiatj <siemiatj@example.com>
Date:   Wed Jul 30 00:34:10 2014 +0200

    foo.txt added

commit 69204cdf0acbab201619d95ad8295928e7f411d5
Author: Kate Hudson <katehudson@example.com>
Date:   Tue Jul 29 13:14:46 2014 -0400

    Fixes #6: Force pushing after amending commits
```

ç°å¨æä»¬ååå°ä¸»(main)åæ¯ï¼âä¸å°å¿çâå é¤`my-branch`åæ¯

```sh
(my-branch)$ git checkout main
Switched to branch 'main'
Your branch is up-to-date with 'origin/main'.
(main)$ git branch -D my-branch
Deleted branch my-branch (was 4e3cd85).
(main)$ echo oh noes, deleted my branch!
oh noes, deleted my branch!
```

å¨è¿æ¶åä½ åºè¯¥æ³èµ·äº`reflog`, ä¸ä¸ªåçº§ççæ¥å¿ï¼å®å­å¨äºä»åº(repo)éé¢ææå¨ä½çåå²ã

```
(main)$ git reflog
69204cd HEAD@{0}: checkout: moving from my-branch to main
4e3cd85 HEAD@{1}: commit: foo.txt added
69204cd HEAD@{2}: checkout: moving from main to my-branch
```

æ­£å¦ä½ æè§ï¼æä»¬æä¸ä¸ªæ¥èªå é¤åæ¯çæäº¤hash(commit hash)ï¼æ¥ä¸æ¥ççæ¯å¦è½æ¢å¤å é¤äºçåæ¯ã

```sh
(main)$ git checkout -b my-branch-help
Switched to a new branch 'my-branch-help'
(my-branch-help)$ git reset --hard 4e3cd85
HEAD is now at 4e3cd85 foo.txt added
(my-branch-help)$ ls
README.md foo.txt
```

ç! æä»¬æå é¤çæä»¶æ¾åæ¥äºã Gitç `reflog` å¨rebasingåºéçæ¶åä¹æ¯åæ ·æç¨çã

<a name="i-want-to-delete-a-branch"></a>
### ææ³å é¤ä¸ä¸ªåæ¯

å é¤ä¸ä¸ªè¿ç¨åæ¯:

```sh
(main)$ git push origin --delete my-branch
```

ä½ ä¹å¯ä»¥:

```sh
(main)$ git push origin :my-branch
```

å é¤ä¸ä¸ªæ¬å°åæ¯:

```sh
(main)$ git branch -D my-branch
```

<a name="i-want-to-checkout-to-a-remote-branch-that-someone-else-is-working-on"></a>
### ææ³ä»å«äººæ­£å¨å·¥ä½çè¿ç¨åæ¯ç­¾åº(checkout)ä¸ä¸ªåæ¯

é¦å, ä»è¿ç¨æå(fetch) ææåæ¯:

```sh
(main)$ git fetch --all
```

åè®¾ä½ æ³è¦ä»è¿ç¨ç`daves`åæ¯ç­¾åºå°æ¬å°ç`daves`

```sh
(main)$ git checkout --track origin/daves
Branch daves set up to track remote branch daves from origin.
Switched to a new branch 'daves'
```

(`--track` æ¯ `git checkout -b [branch] [remotename]/[branch]` çç®å)

è¿æ ·å°±å¾å°äºä¸ä¸ª`daves`åæ¯çæ¬å°æ·è´, ä»»ä½æ¨è¿(pushed)çæ´æ°ï¼è¿ç¨é½è½çå°.

## Rebasing ååå¹¶(Merging)

<a name="undo-rebase"></a>
### ææ³æ¤érebase/merge

ä½ å¯ä»¥åå¹¶(merge)ærebaseäºä¸ä¸ªéè¯¯çåæ¯, æèå®æä¸äºä¸ä¸ªè¿è¡ä¸­çrebase/mergeã Git å¨è¿è¡å±é©æä½çæ¶åä¼æåå§çHEADä¿å­å¨ä¸ä¸ªå«ORIG_HEADçåéé, æä»¥è¦æåæ¯æ¢å¤å°rebase/mergeåçç¶ææ¯å¾å®¹æçã

```sh
(my-branch)$ git reset --hard ORIG_HEAD
```

<a name="force-push-rebase"></a>
### æå·²ç»rebaseè¿, ä½æ¯æä¸æ³å¼ºæ¨(force push)

ä¸å¹¸çæ¯ï¼å¦æä½ æ³æè¿äºåå(changes)ååºå°è¿ç¨åæ¯ä¸ï¼ä½ å°±å¿é¡»å¾å¼ºæ¨(force push)ã æ¯å ä½ å¿«è¿(Fast forward)äºæäº¤ï¼æ¹åäºGitåå², è¿ç¨åæ¯ä¸ä¼æ¥ååå(changes)ï¼é¤éå¼ºæ¨(force push)ãè¿å°±æ¯è®¸å¤äººä½¿ç¨ merge å·¥ä½æµ, èä¸æ¯ rebasing å·¥ä½æµçä¸»è¦åå ä¹ä¸ï¼ å¼åèçå¼ºæ¨(force push)ä¼ä½¿å¤§çå¢éé·å¥éº»ç¦ãä½¿ç¨æ¶éè¦æ³¨æï¼ä¸ç§å®å¨ä½¿ç¨ rebase çæ¹æ³æ¯ï¼ä¸è¦æä½ çåå(changes)åæ å°è¿ç¨åæ¯ä¸, èæ¯æä¸é¢çå:

```sh
(main)$ git checkout my-branch
(my-branch)$ git rebase -i main
(my-branch)$ git checkout main
(main)$ git merge --ff-only my-branch
```

æ´å¤, åè§ [this SO thread](http://stackoverflow.com/questions/11058312/how-can-i-use-git-rebase-without-requiring-a-forced-push).

<a name="interactive-rebase"></a>
### æéè¦ç»å(combine)å ä¸ªæäº¤(commit)

åè®¾ä½ çå·¥ä½åæ¯å°ä¼åå¯¹äº `main` çpull-requestã ä¸è¬æåµä¸ä½ ä¸å³å¿æäº¤(commit)çæ¶é´æ³ï¼åªæ³ç»å *ææ* æäº¤(commit) å°ä¸ä¸ªåç¬çéé¢, ç¶åéç½®(reset)éæäº¤(recommit)ã ç¡®ä¿ä¸»(main)åæ¯æ¯ææ°çåä½ çååé½å·²ç»æäº¤äº, ç¶å:

```sh
(my-branch)$ git reset --soft main
(my-branch)$ git commit -am "New awesome feature"
```

å¦æä½ æ³è¦æ´å¤çæ§å¶, æ³è¦ä¿çæ¶é´æ³, ä½ éè¦åäº¤äºå¼rebase (interactive rebase):

```sh
(my-branch)$ git rebase -i main
```

å¦ææ²¡æç¸å¯¹çå¶å®åæ¯ï¼ ä½ å°ä¸å¾ä¸ç¸å¯¹èªå·±ç`HEAD` è¿è¡ rebaseã ä¾å¦ï¼ä½ æ³ç»åæè¿çä¸¤æ¬¡æäº¤(commit), ä½ å°ç¸å¯¹äº`HEAD~2` è¿è¡rebaseï¼ ç»åæè¿3æ¬¡æäº¤(commit), ç¸å¯¹äº`HEAD~3`, ç­ç­ã

```sh
(main)$ git rebase -i HEAD~2
```

å¨ä½ æ§è¡äºäº¤äºå¼ rebaseçå½ä»¤(interactive rebase command)å, ä½ å°å¨ä½ çç¼è¾å¨éçå°ç±»ä¼¼ä¸é¢çåå®¹:

```vim
pick a9c8a1d Some refactoring
pick 01b2fd8 New awesome feature
pick b729ad5 fixup
pick e3851e8 another fix

# Rebase 8074d12..b729ad5 onto 8074d12
#
# Commands:
#  p, pick = use commit
#  r, reword = use commit, but edit the commit message
#  e, edit = use commit, but stop for amending
#  s, squash = use commit, but meld into previous commit
#  f, fixup = like "squash", but discard this commit's log message
#  x, exec = run command (the rest of the line) using shell
#
# These lines can be re-ordered; they are executed from top to bottom.
#
# If you remove a line here THAT COMMIT WILL BE LOST.
#
# However, if you remove everything, the rebase will be aborted.
#
# Note that empty commits are commented out
```

ææä»¥ `#` å¼å¤´çè¡é½æ¯æ³¨é, ä¸ä¼å½±å rebase.

ç¶åï¼ä½ å¯ä»¥ç¨ä»»ä½ä¸é¢å½ä»¤åè¡¨çå½ä»¤æ¿æ¢ `pick`, ä½ ä¹å¯ä»¥éè¿å é¤å¯¹åºçè¡æ¥å é¤ä¸ä¸ªæäº¤(commit)ã

ä¾å¦, å¦æä½ æ³ **åç¬ä¿çææ§(first)çæäº¤(commit),ç»åææå©ä¸çå°ç¬¬äºä¸ªéé¢**, ä½ å°±åºè¯¥ç¼è¾ç¬¬äºä¸ªæäº¤(commit)åé¢çæ¯ä¸ªæäº¤(commit) åçåè¯ä¸º `f`:

```vim
pick a9c8a1d Some refactoring
pick 01b2fd8 New awesome feature
f b729ad5 fixup
f e3851e8 another fix
```

å¦æä½ æ³ç»åè¿äºæäº¤(commit) **å¹¶éå½åè¿ä¸ªæäº¤(commit)**, ä½ åºè¯¥å¨ç¬¬äºä¸ªæäº¤(commit)æè¾¹æ·»å ä¸ä¸ª`r`ï¼æèæ´ç®åçç¨`s` æ¿ä»£ `f`:

```vim
pick a9c8a1d Some refactoring
pick 01b2fd8 New awesome feature
s b729ad5 fixup
s e3851e8 another fix
```

ä½ å¯ä»¥å¨æ¥ä¸æ¥å¼¹åºçææ¬æç¤ºæ¡ééå½åæäº¤(commit)ã

```vim
Newer, awesomer features

# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
# rebase in progress; onto 8074d12
# You are currently editing a commit while rebasing branch 'main' on '8074d12'.
#
# Changes to be committed:
#	modified:   README.md
#

```

å¦ææåäº, ä½ åºè¯¥çå°ç±»ä¼¼ä¸é¢çåå®¹:

```sh
(main)$ Successfully rebased and updated refs/heads/main.
```

#### å®å¨åå¹¶(merging)ç­ç¥
`--no-commit` æ§è¡åå¹¶(merge)ä½ä¸èªå¨æäº¤, ç»ç¨æ·å¨åæäº¤åæ£æ¥åä¿®æ¹çæºä¼ã `no-ff` ä¼ä¸ºç¹æ§åæ¯(feature branch)çå­å¨è¿çä¸è¯æ®, ä¿æé¡¹ç®åå²ä¸è´ã

```sh
(main)$ git merge --no-ff --no-commit my-branch
```

#### æéè¦å°ä¸ä¸ªåæ¯åå¹¶æä¸ä¸ªæäº¤(commit)

```sh
(main)$ git merge --squash my-branch
```

<a name="rebase-unpushed-commits"></a>
#### æåªæ³ç»å(combine)æªæ¨çæäº¤(unpushed commit)

ææ¶åï¼å¨å°æ°æ®æ¨åä¸æ¸¸ä¹åï¼ä½ æå ä¸ªæ­£å¨è¿è¡çå·¥ä½æäº¤(commit)ãè¿æ¶åä¸å¸ææå·²ç»æ¨(push)è¿çç»åè¿æ¥ï¼å ä¸ºå¶ä»äººå¯è½å·²ç»ææäº¤(commit)å¼ç¨å®ä»¬äºã

```sh
(main)$ git rebase -i @{u}
```

è¿ä¼äº§çä¸æ¬¡äº¤äºå¼çrebase(interactive rebase), åªä¼ååºæ²¡ææ¨(push)çæäº¤(commit)ï¼ å¨è¿ä¸ªåè¡¨æ¶è¿è¡reorder/fix/squash é½æ¯å®å¨çã

<a name="check-if-all-commits-on-a-branch-are-merged"></a>
### æ£æ¥æ¯å¦åæ¯ä¸çæææäº¤(commit)é½åå¹¶(merge)è¿äº

æ£æ¥ä¸ä¸ªåæ¯ä¸çæææäº¤(commit)æ¯å¦é½å·²ç»åå¹¶(merge)å°äºå¶å®åæ¯, ä½ åºè¯¥å¨è¿äºåæ¯çhead(æä»»ä½ commits)ä¹é´åä¸æ¬¡diff:

```sh
(main)$ git log --graph --left-right --cherry-pick --oneline HEAD...feature/120-on-scroll
```

è¿ä¼åè¯ä½ å¨ä¸ä¸ªåæ¯éæèå¦ä¸ä¸ªåæ¯æ²¡æçæææäº¤(commit), ååæ¯ä¹é´ä¸å±äº«çæäº¤(commit)çåè¡¨ã å¦ä¸ä¸ªåæ³å¯ä»¥æ¯:

```sh
(main)$ git log main ^feature/120-on-scroll --no-merges
```

### äº¤äºå¼rebase(interactive rebase)å¯è½åºç°çé®é¢

<a name="noop"></a>
#### è¿ä¸ªrebase ç¼è¾å±å¹åºç°'noop'

å¦æä½ çå°çæ¯è¿æ ·:
```
noop
```

è¿æå³çä½ rebaseçåæ¯åå½ååæ¯å¨åä¸ä¸ªæäº¤(commit)ä¸, æè *é¢å(ahead)* å½ååæ¯ã ä½ å¯ä»¥å°è¯:

* æ£æ¥ç¡®ä¿ä¸»(main)åæ¯æ²¡æé®é¢
* rebase  `HEAD~2` æèæ´æ©

<a name="merge-conflict"></a>
#### æå²çªçæåµ

å¦æä½ ä¸è½æåçå®ærebase, ä½ å¯è½å¿é¡»è¦è§£å³å²çªã

é¦åæ§è¡ `git status` æ¾åºåªäºæä»¶æå²çª:

```sh
(my-branch)$ git status
On branch my-branch
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   README.md
```

å¨è¿ä¸ªä¾å­éé¢, `README.md` æå²çªã æå¼è¿ä¸ªæä»¶æ¾å°ç±»ä¼¼ä¸é¢çåå®¹:

```vim
   <<<<<<< HEAD
   some code
   =========
   some code
   >>>>>>> new-commit
```

ä½ éè¦è§£å³æ°æäº¤çä»£ç (ç¤ºä¾é, ä»ä¸­é´`==`çº¿å°`new-commit`çå°æ¹)ä¸`HEAD` ä¹é´ä¸ä¸æ ·çå°æ¹.

ææ¶åè¿äºåå¹¶éå¸¸å¤æï¼ä½ åºè¯¥ä½¿ç¨å¯è§åçå·®å¼ç¼è¾å¨(visual diff editor):

```sh
(main*)$ git mergetool -t opendiff
```

å¨ä½ è§£å³å®ææå²çªåæµè¯è¿å, `git add` ååäºç(changed)æä»¶, ç¶åç¨`git rebase --continue` ç»§ç»­rebaseã

```sh
(my-branch)$ git add README.md
(my-branch)$ git rebase --continue
```

å¦æå¨è§£å³å®ææçå²çªè¿åï¼å¾å°äºä¸æäº¤åä¸æ ·çç»æ, å¯ä»¥æ§è¡`git rebase --skip`ã

ä»»ä½æ¶åä½ æ³ç»ææ´ä¸ªrebase è¿ç¨ï¼åæ¥rebaseåçåæ¯ç¶æ, ä½ å¯ä»¥å:

```sh
(my-branch)$ git rebase --abort
```

<a name="stashing"></a>
## Stash

### æå­æææ¹å¨

æå­ä½ å·¥ä½ç®å½ä¸çæææ¹å¨

```sh
$ git stash
```

ä½ å¯ä»¥ä½¿ç¨`-u`æ¥æé¤ä¸äºæä»¶

```sh
$ git stash -u
```

### æå­æå®æä»¶

åè®¾ä½ åªæ³æå­æä¸ä¸ªæä»¶

```sh
$ git stash push working-directory-path/filename.ext
```

åè®¾ä½ æ³æå­å¤ä¸ªæä»¶

```sh
$ git stash push working-directory-path/filename1.ext working-directory-path/filename2.ext
```

<a name="stash-msg"></a>
### æå­æ¶è®°å½æ¶æ¯

è¿æ ·ä½ å¯ä»¥å¨`list`æ¶çå°å®

```sh
$ git stash save <message>
```
æ
```sh
$ git stash push -m <message>
```
<a name="stash-apply-specific"></a>
### ä½¿ç¨æä¸ªæå®æå­

é¦åä½ å¯ä»¥æ¥çä½ ç`stash`è®°å½

```sh
$ git stash list
```

ç¶åä½ å¯ä»¥`apply`æä¸ª`stash`

```sh
$ git stash apply "stash@{n}"
```

æ­¤å¤ï¼ 'n'æ¯`stash`å¨æ ä¸­çä½ç½®ï¼æä¸å±ç`stash`ä¼æ¯0

é¤æ­¤ä¹å¤ï¼ä¹å¯ä»¥ä½¿ç¨æ¶é´æ è®°(åå¦ä½ è½è®°å¾çè¯)ã

```sh
$ git stash apply "stash@{2.hours.ago}"
```

<a href="stage-and-keep-unstaged"></a>
### æå­æ¶ä¿çæªæå­çåå®¹

ä½ éè¦æå¨createä¸ä¸ª`stash commit`ï¼ ç¶åä½¿ç¨`git stash store`ã

```sh
$ git stash create
$ git stash store -m "commit-message" CREATED_SHA1
```

<a name="miscellaneous-objects"></a>
## æé¡¹(Miscellaneous Objects)

<a name="clone-submodules"></a>
### åéææå­æ¨¡å

```sh
$ git clone --recursive git://github.com/foo/bar.git
```

å¦æå·²ç»åéäº:

```sh
$ git submodule update --init --recursive
```

<a name="delete-tag"></a>
### å é¤æ ç­¾(tag)

```sh
$ git tag -d <tag_name>
$ git push <remote> :refs/tags/<tag_name>
```

<a name="recover-tag"></a>
### æ¢å¤å·²å é¤æ ç­¾(tag)

å¦æä½ æ³æ¢å¤ä¸ä¸ªå·²å é¤æ ç­¾(tag), å¯ä»¥æç§ä¸é¢çæ­¥éª¤: é¦å, éè¦æ¾å°æ æ³è®¿é®çæ ç­¾(unreachable tag):

```sh
$ git fsck --unreachable | grep tag
```

è®°ä¸è¿ä¸ªæ ç­¾(tag)çhashï¼ç¶åç¨Gitç [update-ref](http://git-scm.com/docs/git-update-ref):

```sh
$ git update-ref refs/tags/<tag_name> <hash>
```

è¿æ¶ä½ çæ ç­¾(tag)åºè¯¥å·²ç»æ¢å¤äºã

<a name="deleted-patch"></a>
### å·²å é¤è¡¥ä¸(patch)

å¦ææäººå¨ GitHub ä¸ç»ä½ åäºä¸ä¸ªpull request, ä½æ¯ç¶åä»å é¤äºä»èªå·±çåå§ fork, ä½ å°æ²¡æ³åéä»ä»¬çæäº¤(commit)æä½¿ç¨ `git am`ãå¨è¿ç§æåµä¸, æå¥½æå¨çæ¥çä»ä»¬çæäº¤(commit)ï¼å¹¶æå®ä»¬æ·è´å°ä¸ä¸ªæ¬å°æ°åæ¯ï¼ç¶ååæäº¤ã

åå®æäº¤å, åä¿®æ¹ä½èï¼åè§[åæ´ä½è](#commit-wrong-author)ã ç¶å, åºç¨åå, ååèµ·ä¸ä¸ªæ°çpull requestã

## è·è¸ªæä»¶(Tracking Files)

<a href="i-want-to-change-a-file-names-capitalization-without-changing-the-contents-of-the-file"></a>
### æåªæ³æ¹åä¸ä¸ªæä»¶åå­çå¤§å°åï¼èä¸ä¿®æ¹åå®¹

```sh
(main)$ git mv --force myfile MyFile
```

<a href="remove-from-git"></a>
### ææ³ä»Gitå é¤ä¸ä¸ªæä»¶ï¼ä½ä¿çè¯¥æä»¶

```sh
(main)$ git rm --cached log.txt
```

## éç½®(Configuration)

<a name="adding-command-aliases"></a>
### ææ³ç»ä¸äºGitå½ä»¤æ·»å å«å(alias)

å¨ OS X å Linux ä¸, ä½ ç Gitçéç½®æä»¶å¨å­å¨ ```~/.gitconfig```ãæå¨```[alias]``` é¨åæ·»å äºä¸äºå¿«æ·å«å(åä¸äºæå®¹ææ¼åéè¯¯ç)ï¼å¦ä¸:

```vim
[alias]
    a = add
    amend = commit --amend
    c = commit
    ca = commit --amend
    ci = commit -a
    co = checkout
    d = diff
    dc = diff --changed
    ds = diff --staged
    f = fetch
    loll = log --graph --decorate --pretty=oneline --abbrev-commit
    m = merge
    one = log --pretty=oneline
    outstanding = rebase -i @{u}
    s = status
    unpushed = log @{u}
    wc = whatchanged
    wip = rebase -i @{u}
    zap = fetch -p
```

<a name="credential-helper"></a>
### ææ³ç¼å­ä¸ä¸ªä»åº(repository)çç¨æ·ååå¯ç 

ä½ å¯è½æä¸ä¸ªä»åºéè¦ææï¼è¿æ¶ä½ å¯ä»¥ç¼å­ç¨æ·ååå¯ç ï¼èä¸ç¨æ¯æ¬¡æ¨/æ(push/pull)çæ¶åé½è¾å¥ï¼Credential helperè½å¸®ä½ ã

```sh
$ git config --global credential.helper cache
# Set git to use the credential memory cache
```

```sh
$ git config --global credential.helper 'cache --timeout=3600'
# Set the cache to timeout after 1 hour (setting is in seconds)
```

<a href="#ive-no-idea-what-i-did-wrong"></a>
## æä¸ç¥éæåéäºäºä»ä¹

ä½ æäºææç ¸äºï¼ä½  `éç½®(reset)` äºä¸äºä¸è¥¿, æèä½ åå¹¶äºéè¯¯çåæ¯, äº¦æä½ å¼ºæ¨äºåæ¾ä¸å°ä½ èªå·±çæäº¤(commit)äºãæäºæ¶å, ä½ ä¸ç´é½åå¾å¾å¥½, ä½ä½ æ³åå°ä»¥åçæä¸ªç¶æã

è¿å°±æ¯ `git reflog` çç®çï¼ `reflog` è®°å½å¯¹åæ¯é¡¶ç«¯(the tip of a branch)çä»»ä½æ¹å, å³ä½¿é£ä¸ªé¡¶ç«¯æ²¡æè¢«ä»»ä½åæ¯ææ ç­¾å¼ç¨ãåºæ¬ä¸, æ¯æ¬¡HEADçæ¹å, ä¸æ¡æ°çè®°å½å°±ä¼å¢å å°`reflog`ãéæ¾çæ¯ï¼è¿åªå¯¹æ¬å°åæ¯èµ·ä½ç¨ï¼ä¸å®åªè·è¸ªå¨ä½ (ä¾å¦ï¼ä¸ä¼è·è¸ªä¸ä¸ªæ²¡æè¢«è®°å½çæä»¶çä»»ä½æ¹å)ã

```sh
(main)$ git reflog
0a2e358 HEAD@{0}: reset: moving to HEAD~2
0254ea7 HEAD@{1}: checkout: moving from 2.2 to main
c10f740 HEAD@{2}: checkout: moving from main to 2.2
```

ä¸é¢çreflogå±ç¤ºäºä»mainåæ¯ç­¾åº(checkout)å°2.2 åæ¯ï¼ç¶ååç­¾åã é£éï¼è¿æä¸ä¸ªç¡¬éç½®(hard reset)å°ä¸ä¸ªè¾æ§çæäº¤ãææ°çå¨ä½åºç°å¨æä¸é¢ä»¥ `HEAD@{0}`æ è¯.

å¦æäºå®è¯æä½ ä¸å°å¿åç§»(move back)äºæäº¤(commit), reflog ä¼åå«ä½ ä¸å°å¿åç§»åmainä¸æåçæäº¤(0254ea7)ã

```sh
$ git reset --hard 0254ea7
```

ç¶åä½¿ç¨git resetå°±å¯ä»¥æmainæ¹åå°ä¹åçcommitï¼è¿æä¾äºä¸ä¸ªå¨åå²è¢«æå¤æ´æ¹æåµä¸çå®å¨ç½ã

([æèª](https://www.atlassian.com/git/tutorials/rewriting-history/git-reflog)).

# å¶å®èµæº(Other Resources)

## ä¹¦(Books)

* [Pro Git](https://git-scm.com/book/en/v2) - Scott Chacon's excellent git book
* [Git Internals](https://github.com/pluralsight/git-internals-pdf) - Scott Chacon's other excellent git book

## æç¨(Tutorials)

* [Learn Git branching](https://learngitbranching.js.org/) ä¸ä¸ªåºäºç½é¡µçäº¤äºå¼ branching/merging/rebasing æç¨
* [Getting solid at Git rebase vs. merge](https://medium.com/@porteneuve/getting-solid-at-git-rebase-vs-merge-4fa1a48c53aa)
* [git-workflow](https://github.com/asmeurer/git-workflow) - [Aaron Meurer](https://github.com/asmeurer)çæä¹ä½¿ç¨Gitä¸ºå¼æºä»åºè´¡ç®
* [GitHub as a workflow](http://hugogiraudel.com/2015/08/13/github-as-a-workflow/) - ä½¿ç¨GitHubåä¸ºå·¥ä½æµçè¶£äº, å°¤å¶æ¯ç©ºPRs

## èæ¬åå·¥å·(Scripts and Tools)

* [firstaidgit.io](http://firstaidgit.io/) ä¸ä¸ªå¯æç´¢çæå¸¸è¢«é®å°çGitçé®é¢
* [git-extra-commands](https://github.com/unixorn/git-extra-commands) - ä¸å æç¨çé¢å¤çGitèæ¬
* [git-extras](https://github.com/tj/git-extras) - GIT å·¥å·é -- repo summary, repl, changelog population, author commit percentages and more
* [git-fire](https://github.com/qw3rtman/git-fire) - git-fire æ¯ä¸ä¸ª Git æä»¶ï¼ç¨äºå¸®å©å¨ç´§æ¥æåµä¸æ·»å ææå½åæä»¶, åæäº¤(committing), åæ¨(push)å°ä¸ä¸ªæ°åæ¯(é»æ­¢åå¹¶å²çª)ã
* [git-tips](https://github.com/git-tips/tips) - Gitå°æç¤º
* [git-town](https://github.com/Originate/git-town) - éç¨ï¼é«çº§Gitå·¥ä½æµæ¯æï¼ http://www.git-town.com

## GUIå®¢æ·ç«¯(GUI Clients)
* [GitKraken](https://www.gitkraken.com/) - è±ªåçGitå®¢æ·ç«¯ Windows, Mac & Linux
* [git-cola](https://git-cola.github.io/) - å¦å¤ä¸ä¸ªGitå®¢æ·ç«¯ Windows & OS X
* [GitUp](https://github.com/git-up/GitUp) - ä¸ä¸ªæ°çGitå®¢æ·ç«¯ï¼å¨å¤çGitçå¤ææ§ä¸æèªå·±çç¹ç¹
* [gitx-dev](https://rowanj.github.io/gitx/) - å¾å½¢åçGitå®¢æ·ç«¯ OS X
* [Source Tree](https://www.sourcetreeapp.com/) - åè´¹çå¾å½¢åGitå®¢æ·ç«¯ Windows & OS X
* [Tower](http://www.git-tower.com/) - å¾å½¢åGitå®¢æ·ç«¯ OS X(ä»è´¹)
