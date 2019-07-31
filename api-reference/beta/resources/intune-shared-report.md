---
title: Tipo de recurso report
description: Descreve o recurso de relatório da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c27df6cb965e4be5c186ee8bf14a65e467f538b4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010389"
---
# <a name="report-resource-type"></a>Tipo de recurso report

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Retorna o conteúdo apropriado para o contexto, incluindo:

- Relatórios de histórico de perfil de configuração de dispositivo.
- Relatórios de falha de registro.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conteúdo|Fluxo|Conteúdo de relatórios; os detalhes variam por tipo de relatório.|

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



