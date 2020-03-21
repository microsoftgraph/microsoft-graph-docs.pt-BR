---
title: tipo de recurso de impressora
description: Representa um dispositivo de impressora física que foi registrado com o serviço de impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações da impressora, metadados da impressora e status do registro.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c1d8805e54a194eeb584bb980ed8082502b4a872
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895504"
---
# <a name="printer-resource-type"></a>tipo de recurso de impressora

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um dispositivo de impressora física que foi registrado com o serviço de impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações da impressora, metadados da impressora e status do registro.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter impressora](../api/printer-get.md) | [impressora](printer.md) | Leia as propriedades e as relações do objeto Printer. |
| [Update](../api/printer-update.md) | [impressora](printer.md) | Atualize o objeto Printer. |
| [Delete](../api/printer-delete.md) | Nenhum | Cancelar o registro do printerfrom físico o serviço de impressão universal. |
| [getCapabilities](../api/printer-getcapabilities.md) | [printerCapabilities](printercapabilities.md) | Obtenha uma lista de recursos para a impressora. |
| [resetDefaults](../api/printer-resetdefaults.md) | Nenhum | Redefinir as configurações padrão de uma impressora. |
| [Listar trabalhos](../api/printer-list-jobs.md) | coleção [printJob](printjob.md) | Obtenha uma lista de trabalhos de impressão que são enfileirados para processamento pela impressora. |
| [Criar trabalho](../api/printer-post-jobs.md) | [Impressão](printjob.md) | Crie um novo trabalho de impressão para a impressora. Para começar a imprimir o trabalho, use [startPrintJob](../api/printjob-startprintjob.md). |
| [Conectores de lista](../api/printer-list-connectors.md) | coleção [Multiconnector](printconnector.md) | Obter uma lista de conectores aos quais esta impressora está associada. |
| [Listar allowedUsers](../api/printer-list-allowedusers.md) | coleção [UserIdentity](useridentity.md) | Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para a impressora associada. |
| [Adicionar allowedUser](../api/printer-post-allowedusers.md) | Nenhum | Conceda ao usuário especificado acesso para enviar trabalhos de impressão à impressora associada. |
| [Remover allowedUser](../api/printer-delete-alloweduser.md) | Nenhum | Revogar o acesso à impressora do usuário especificado. |
| [Listar allowedGroups](../api/printer-list-allowedgroups.md) | coleção [Identity](identity.md) | Recupere uma lista de grupos aos quais foi concedido acesso para enviar trabalhos de impressão à impressora associada. |
| [Adicionar o permitido](../api/printer-post-allowedgroups.md) | Nenhum | Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão à impressora associada. |
| [Remover o permitido](../api/printer-delete-allowedgroup.md) | Nenhum | Revogar o acesso à impressora do grupo especificado. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador do documento. Somente leitura.|
|name|String|O nome da impressora.|
|fabricante|String|O fabricante relatado pela impressora. Somente leitura.|
|modelo|String|O nome do modelo relatado pela impressora. Somente leitura.|
|registeredBy|[userIdentity](useridentity.md)|O usuário que registrou a impressora.|
|registeredDateTime|DateTimeOffset|O DateTimeOffset quando a impressora foi registrada. Somente leitura.|
|status|[printerStatus](printerstatus.md)|O status de processamento da impressora, incluindo erros. Somente leitura.|
|isShared|Booliano|True se a impressora é compartilhada; caso contrário, false. Somente leitura.|
|acceptingJobs|Boolean|Se a impressora está atualmente aceitando novos trabalhos de impressão.|
|location|[printerLocation](printerlocation.md)|O local físico e/ou organizacional da impressora.|
|padrões|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão da impressora.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|serviços|coleção [printJob](printjob.md)| A lista de trabalhos que estão na fila para impressão pela impressora. Somente leitura. Anulável.|
|shares|[printerShare](printershare.md)| O printerShare associado à impressora. Somente leitura. Anulável.|
|conectores|[separador de Hiperligação](printconnector.md)|Os conectores associados à impressora.|
|allowedUsers|coleção [UserIdentity](useridentity.md)|Os usuários que têm acesso à impressão usando a impressora.|
|allowedGroups|[identity](identity.md)|Os grupos cujos usuários têm acesso para imprimir usando a impressora.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printer",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "acceptingJobs": true,
  "registeredBy": {"@odata.type": "microsoft.graph.userIdentity"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->