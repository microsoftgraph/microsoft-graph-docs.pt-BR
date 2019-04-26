---
title: tipo de enumeração edgeTelemetryMode
description: Tipo de dados de navegação enviados para a análise do Microsoft 365
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d671849e34d27403450ae6324b824a92ae9d9b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566035"
---
# <a name="edgetelemetrymode-enum-type"></a>tipo de enumeração edgeTelemetryMode

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de dados de navegação enviados para a análise do Microsoft 365

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Padrão – nenhum dado de telemetria coletado ou enviado|
|Internet|1 |Permitir o envio de histórico de intranet somente: enviar apenas dados de histórico de navegação para sites de intranet|
|provedor|2 |Permitir o envio somente do histórico da Internet: Enviar somente dados de histórico de navegação para sites da Internet|
|intranetAndInternet|3 |Permitir o envio do histórico de intranet e Internet: enviar dados de histórico de navegação para sites de intranet e Internet|





