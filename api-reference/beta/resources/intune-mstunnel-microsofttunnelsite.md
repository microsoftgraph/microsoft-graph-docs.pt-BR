---
title: Tipo de recurso microsoftTunnelSite
description: Entidade que representa um Microsoft Tunnel site
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de026e42f21b29327620f3170fa4d3e8117af01342b0e494bafa949efb1c8261
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178861"
---
# <a name="microsofttunnelsite-resource-type"></a>Tipo de recurso microsoftTunnelSite

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um Microsoft Tunnel site

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftTunnelSites](../api/intune-mstunnel-microsofttunnelsite-list.md)|[Coleção microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Listar propriedades e relações dos [objetos microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Obter microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-get.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Leia propriedades e relações do [objeto microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Criar microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-create.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Crie um novo [objeto microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Excluir microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-delete.md)|Nenhum|Exclui um [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md).|
|[Atualizar microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-update.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Atualize as propriedades de um [objeto microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Id do MicrosoftTunnelSite|
|displayName|Cadeia de caracteres|O nome de exibição do MicrosoftTunnelSite|
|description|Cadeia de caracteres|Descrição do MicrosoftTunnelSite|
|publicAddress|Cadeia de caracteres|O nome de domínio público do MicrosoftTunnelSite ou o endereço IP|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta instância entity.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|microsoftTunnelConfiguration|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|O MicrosoftTunnelConfiguration que foi aplicado a este MicrosoftTunnelSite|
|microsoftTunnelServers|[Coleção microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Uma lista de MicrosoftTunnelServers que estão registrados neste MicrosoftTunnelSite|

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




