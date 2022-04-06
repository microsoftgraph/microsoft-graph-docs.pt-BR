---
title: Tipo de recurso customAccessPackageWorkflowExtension
description: Define os atributos de um aplicativo lógico, que pode ser chamado em vários estágios de uma solicitação de pacote de acesso e ciclo de atribuição.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b89d41ec573d6035e19590d7015df4e7269909f3
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672732"
---
# <a name="customaccesspackageworkflowextension-resource-type"></a>Tipo de recurso customAccessPackageWorkflowExtension

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define os atributos de um aplicativo lógico, que pode ser chamado em vários estágios de uma solicitação de pacote de acesso e ciclo de atribuição. Você pode integrar aplicativos lógicos com o gerenciamento de direitos para ampliar seus fluxos de trabalho de governança além dos principais casos de uso do gerenciamento de direitos. Os seguintes casos de uso podem ser integrados a aplicativos lógicos usando este fluxo de trabalho:
- Quando um [pacote de acesso é solicitado](accesspackageassignmentrequest.md)
- Quando uma [solicitação de pacote de acesso é concedida](accesspackageassignment.md)
- Quando uma [atribuição de pacote de acesso expira](accesspackageassignment.md)

Herda e derivado de [customCalloutExtension](../resources/customcalloutextension.md).


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-list-customaccesspackageworkflowextensions.md)|[coleção customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Obter uma lista dos [objetos customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) e suas propriedades.|
|[Criar customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-post-customaccesspackageworkflowextensions.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Crie um novo [objeto customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Obter customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-get.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Leia as propriedades e as relações de um [objeto customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Atualizar customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-update.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Atualize as propriedades de [um objeto customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Excluir customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-delete.md)|Nenhum|Exclui um [objeto customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|authenticationConfiguration|[customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md)|Configuração para proteger a chamada da API para o aplicativo lógico. Por exemplo, o fluxo de credenciais do cliente OAuth. Herdado [de customCalloutExtension](../resources/customcalloutextension.md).|
|clientConfiguration|[customExtensionClientConfiguration](../resources/customextensionclientconfiguration.md)| Configurações de conexão HTTP que definem por quanto tempo o Azure AD pode esperar por uma conexão com um aplicativo lógico, quantas vezes você pode repetir uma conexão com tempo de espera e os cenários de exceção quando as recuperações são permitidas. Herdado [de customCalloutExtension](../resources/customcalloutextension.md).|
|createdDateTime|DateTimeOffset|Representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|description|String|Descrição do objeto customAccessPackageWorkflowExtension. Herdado [de customCalloutExtension](../resources/customcalloutextension.md). Somente leitura.|
|displayName|String|Nome para exibição do objeto customAccessPackageWorkflowExtension. Herdado [de customCalloutExtension](../resources/customcalloutextension.md). Somente leitura. Suporta `$filter` (`contains`).|
|endpointConfiguration|[customExtensionEndpointConfiguration](../resources/customextensionendpointconfiguration.md)|O tipo e os detalhes para configurar o ponto de extremidade para chamar o fluxo de trabalho do aplicativo lógico. Herdado [de customCalloutExtension](../resources/customcalloutextension.md).|  
|id|String|Identificador do objeto customAccessPackageWorkflowExtension. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customAccessPackageWorkflowExtension",
  "baseType": "microsoft.graph.customCalloutExtension",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customAccessPackageWorkflowExtension",
  "id": "String (identifier)",
  "displayName": "String",
  "clientConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionClientConfiguration"
  },
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionAuthenticationConfiguration"
  },
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "endpointConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionEndpointConfiguration"
  }
}
```
