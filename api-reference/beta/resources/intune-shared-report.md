---
title: Tipo de recurso report
description: Descreve o recurso de relatório da API Microsoft Graph para Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 098c20b2460324c4975533902e1b71fde1af41c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407470"
---
# <a name="report-resource-type"></a>Tipo de recurso report

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Retorna o conteúdo apropriada para o contexto, incluindo:

- Relatórios de histórico de perfil de configuração de dispositivo.
- Relatórios de falha de inscrição.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|content|Fluxo|Relatório de conteúdo; detalhes variam de acordo com o tipo de relatório.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



