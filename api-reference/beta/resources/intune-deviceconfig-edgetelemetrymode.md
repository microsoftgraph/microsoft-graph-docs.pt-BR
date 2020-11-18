---
title: tipo de enumeração edgeTelemetryMode
description: Tipo de dados de navegação enviados para a análise do Microsoft 365
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9a2ad7e97f9d957e4da278dad6dde3f686445e1a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198878"
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
|Internet|1|Permitir o envio de histórico de intranet somente: enviar apenas dados de histórico de navegação para sites de intranet|
|provedor|duas|Permitir o envio somente do histórico da Internet: Enviar somente dados de histórico de navegação para sites da Internet|
|intranetAndInternet|3D|Permitir o envio do histórico de intranet e Internet: enviar dados de histórico de navegação para sites de intranet e Internet|




