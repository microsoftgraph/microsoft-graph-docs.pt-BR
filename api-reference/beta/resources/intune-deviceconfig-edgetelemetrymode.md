---
title: Tipo denum edgeTelemetryMode
description: Tipo de dados de navegação enviados para Microsoft 365 análise
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0e81e7ccb58db94851e2c56b269dc25050a8c35d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59009172"
---
# <a name="edgetelemetrymode-enum-type"></a>Tipo denum edgeTelemetryMode

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de dados de navegação enviados para Microsoft 365 análise

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Padrão – Sem dados de telemetria coletados ou enviados|
|intranet|1|Permitir apenas o envio de histórico da intranet: enviar apenas dados de histórico de navegação para sites de intranet|
|internet|2|Permitir apenas o envio de histórico da Internet: enviar apenas dados de histórico de navegação para sites da Internet|
|intranetAndInternet|3|Permitir o envio de histórico da intranet e da Internet: Enviar dados de histórico de navegação para intranet e sites da Internet|



