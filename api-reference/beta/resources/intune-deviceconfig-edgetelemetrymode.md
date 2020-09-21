---
title: tipo de enumeração edgeTelemetryMode
description: Tipo de dados de navegação enviados para a análise do Microsoft 365
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5ceb31c9a82fe2d13668aaf5db32b65beba88f26
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016265"
---
# <a name="edgetelemetrymode-enum-type"></a>tipo de enumeração edgeTelemetryMode

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de dados de navegação enviados para a análise do Microsoft 365

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Padrão – nenhum dado de telemetria coletado ou enviado|
|Internet|1 |Permitir o envio de histórico de intranet somente: enviar apenas dados de histórico de navegação para sites de intranet|
|provedor|2 |Permitir o envio somente do histórico da Internet: Enviar somente dados de histórico de navegação para sites da Internet|
|intranetAndInternet|3 |Permitir o envio do histórico de intranet e Internet: enviar dados de histórico de navegação para sites de intranet e Internet|






