---
title: tipo de recurso compartilhado
description: 'Uma compreensão dos representando arquivos compartilhados com ou por um usuário específico. Há suporte para os seguintes arquivos compartilhados:'
ms.openlocfilehash: 786e3cc94a3c108b30cca880491dab5725014570
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038111"
---
# <a name="shared-resource-type"></a>tipo de recurso compartilhado

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma compreensão dos representando arquivos compartilhados com ou por um usuário específico. Há suporte para os seguintes arquivos compartilhados:

- Arquivos anexados diretamente em um email ou uma reunião convidem.
- OneDrive para Bussiness e SharePoint modernos anexos - arquivos armazenados no OneDrive para negócios e do SharePoint que os usuários compartilhem como links em um email.

**Observação**: estamos atualmente trabalhando em preencher os resultados da API compartilhados com dados. Pode haver alguns dados ausentes nas semanas primeira depois do lançamento.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Lista compartilhada](../api/insights-list-shared.md) |coleção [insights_shared](insights-shared.md)| Obtenha uma lista de arquivos compartilhados.|

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                      | Descrição  |
| -------------         |---------------            | -------------|
| id                    | String                    | Identificador exclusivo do relacionamento. Somente leitura.        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | Detalhes sobre o item compartilhado. Somente leitura.        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Propriedades que você pode usar para visualizar o documento na sua experiência. Somente leitura      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Propriedades de referência do documento compartilhado, como a url e o tipo de documento. Somente leitura       |

## <a name="relationships"></a>Relações

| Propriedade      | Tipo          | Descrição  |
| ------------- |---------------| -------------|
| recurso      | Entidade        | Usado para navegar até o item que foi compartilhado. Anexos de arquivo, o tipo é *fileAttachment*. Anexos vinculados, o tipo é *driveItem*. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```