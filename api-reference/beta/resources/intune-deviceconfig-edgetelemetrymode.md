---
title: Tipo denum edgeTelemetryMode
description: Tipo de dados de navegação enviados para Microsoft 365 análise
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c6348746877f20bfab2ce019e37e9a014182235e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805742"
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



