---
title: tipo de recurso microsoftTunnelSite
description: Entidade que representa um site de encapsulamento da Microsoft
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 730d0075009b605db5e132412bddfbf0f58251a6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301439"
---
# <a name="microsofttunnelsite-resource-type"></a>tipo de recurso microsoftTunnelSite

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um site de encapsulamento da Microsoft

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftTunnelSites](../api/intune-mstunnel-microsofttunnelsite-list.md)|coleção [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Listar Propriedades e relações dos objetos [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) .|
|[Obter microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-get.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Leia as propriedades e as relações do objeto [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) .|
|[Criar microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-create.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Criar um novo objeto [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) .|
|[Excluir microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-delete.md)|Nenhum|Exclui [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md).|
|[Atualizar microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-update.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Atualiza as propriedades de um objeto [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID do MicrosoftTunnelSite|
|displayName|String|O nome de exibição do MicrosoftTunnelSite|
|description|String|A descrição do MicrosoftTunnelSite|
|publicAddress|String|O nome de domínio público ou endereço IP do MicrosoftTunnelSite|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|microsoftTunnelConfiguration|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|O MicrosoftTunnelConfiguration que foi aplicado a este MicrosoftTunnelSite|
|microsoftTunnelServers|coleção [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Uma lista de MicrosoftTunnelServers registradas para este MicrosoftTunnelSite|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelSite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publicAddress": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




