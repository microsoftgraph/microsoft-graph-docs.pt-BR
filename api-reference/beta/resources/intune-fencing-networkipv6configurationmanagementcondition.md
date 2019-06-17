---
title: tipo de recurso networkIPv6ConfigurationManagementCondition
description: As condições de gerenciamento baseado em configuração IPv6 podem ser definidas que serão acionadas quando um dispositivo detectar determinadas configurações de rede IP. Uma condição de gerenciamento de configuração IP só será considerada TRUE quando a conexão de rede estiver ativa. Os endereços do servidor DHCP IPv6 podem não ser correspondentes. Isso ocorre porque o Windows (circa Redstone) não expõe essas informações para o serviço de autenticação natural.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 665bbd4cb27d533a230614a2712943c23d1b3d76
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979134"
---
# <a name="networkipv6configurationmanagementcondition-resource-type"></a>tipo de recurso networkIPv6ConfigurationManagementCondition

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

As condições de gerenciamento baseado em configuração IPv6 podem ser definidas que serão acionadas quando um dispositivo detectar determinadas configurações de rede IP. Uma condição de gerenciamento de configuração IP só será considerada TRUE quando a conexão de rede estiver ativa.
Os endereços do servidor DHCP IPv6 podem não ser correspondentes. Isso ocorre porque o Windows (circa Redstone) não expõe essas informações para o serviço de autenticação natural.


Herda de [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar networkIPv6ConfigurationManagementConditions](../api/intune-fencing-networkipv6configurationmanagementcondition-list.md)|coleção [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Listar Propriedades e relações dos objetos [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|
|[Obter networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-get.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Leia as propriedades e as relações do objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|
|[Criar networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-create.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Criar um novo objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|
|[Excluir networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-delete.md)|Nenhum|Exclui [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).|
|[Atualizar networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-update.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Atualiza as propriedades de um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da condição de gerenciamento. Valor gerado pelo sistema atribuído quando criado. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|String|Nome exclusivo para a condição de gerenciamento. Usado em expressões de condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|O nome do administrador definido da condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|descrição|String|A descrição definida pelo administrador da condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi criada. Lado do serviço gerado. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi modificada pela última vez. Atualizado o lado do serviço. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag da condição de gerenciamento. Atualizado o lado do serviço. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|As plataformas aplicáveis para essa condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|ipV6Prefix|String|A sub-rede IPv6 a ser conectada. por exemplo, 2001: DB8::/32|
|ipV6Gateway|String|O endereço do gateway IPv6 para. por exemplo, 2001: DB8:: 1|
|ipV6DNSServerList|Coleção de cadeias de caracteres|Servidores DNS IPv6 configurados para o adaptador.|
|dnsSuffixList|Coleção de cadeias de caracteres|Sufixos DNS válidos para a rede atual. por exemplo, seattle.contoso.com|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managementConditionStatements|coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|As instruções de condição de gerenciamento associadas à condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkIPv6ConfigurationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "ipV6Prefix": "String",
  "ipV6Gateway": "String",
  "ipV6DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```





