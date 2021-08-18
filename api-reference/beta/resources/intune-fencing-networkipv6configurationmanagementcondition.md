---
title: Tipo de recurso networkIPv6ConfigurationManagementCondition
description: As condições de gerenciamento baseadas em configuração IPv6 podem ser definidas que dispararão quando um dispositivo detectar determinadas configurações de rede IP. Uma condição de gerenciamento de configuração de IP só será considerada TRUE quando a conexão de rede estiver ativa. Os endereços de servidor DHCP IPv6 podem não ser corresponder. Isso acontece porque Windows(circa Redstone) não expõe essas informações ao serviço de Autenticação Natural.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f81e5de80585e8cd8f16bb1520132d06074e957
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262190"
---
# <a name="networkipv6configurationmanagementcondition-resource-type"></a>Tipo de recurso networkIPv6ConfigurationManagementCondition

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

As condições de gerenciamento baseadas em configuração IPv6 podem ser definidas que dispararão quando um dispositivo detectar determinadas configurações de rede IP. Uma condição de gerenciamento de configuração de IP só será considerada TRUE quando a conexão de rede estiver ativa.
Os endereços de servidor DHCP IPv6 podem não ser corresponder. Isso acontece porque Windows(circa Redstone) não expõe essas informações ao serviço de Autenticação Natural.


Herda de [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar networkIPv6ConfigurationManagementConditions](../api/intune-fencing-networkipv6configurationmanagementcondition-list.md)|[coleção networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Listar propriedades e relações dos [objetos networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|
|[Obter networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-get.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Leia propriedades e relações do [objeto networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|
|[Criar networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-create.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Crie um novo [objeto networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|
|[Excluir networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-delete.md)|Nenhum|Exclui uma [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).|
|[Atualizar networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-update.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Atualize as propriedades de [um objeto networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da condição de gerenciamento. Valor gerado pelo sistema atribuído quando criado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|Nome único|Cadeia de caracteres|Nome exclusivo para a condição de gerenciamento. Usado em expressões de condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Cadeia de caracteres|O nome definido pelo administrador da condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|Cadeia de caracteres|A descrição definida pelo administrador da condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi criada. Lado de serviço gerado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|O tempo em que a condição de gerenciamento foi modificada pela última vez. Lado do serviço atualizado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag da condição de gerenciamento. Lado do serviço atualizado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[Coleção devicePlatformType](../resources/intune-fencing-deviceplatformtype.md)|As plataformas aplicáveis para essa condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|ipV6Prefix|Cadeia de caracteres|A sub-rede IPv6 a ser conectada. por exemplo, 2001:db8::/32|
|ipV6Gateway|Cadeia de caracteres|O endereço de gateway IPv6 para. por exemplo, 2001:db8::1|
|ipV6DNSServerList|String collection|Um servidor DNS IPv6 configurado para o adaptador.|
|dnsSuffixList|String collection|Sufixos DNS válidos para a rede atual. por exemplo, seattle.contoso.com|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managementConditionStatements|[coleção managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|As instruções de condição de gerenciamento associadas à condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|

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




