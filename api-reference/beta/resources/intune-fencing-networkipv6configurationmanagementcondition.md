---
title: tipo de recurso de networkIPv6ConfigurationManagementCondition
description: Configurações de rede IPv6 condições de gerenciamento baseadas na configuração podem ser definidas que acionará quando um dispositivo detecta certo IP. Uma condição de gerenciamento de configuração IP só será considerada TRUE quando a conexão de rede estiver ativo.
author: tfitzmac
ms.openlocfilehash: de74fddad090993f6829180ba6f5eaea9cdaf59a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305737"
---
# <a name="networkipv6configurationmanagementcondition-resource-type"></a>tipo de recurso de networkIPv6ConfigurationManagementCondition

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configurações de rede IPv6 condições de gerenciamento baseadas na configuração podem ser definidas que acionará quando um dispositivo detecta certo IP. Uma condição de gerenciamento de configuração IP só será considerada TRUE quando a conexão de rede estiver ativo.
Endereços de servidor DHCP IPv6 não podem ser correspondidos. Isso ocorre porque o Windows (aproximadamente em Redstone) não expõe essas informações para o serviço de autenticação Natural.

Herda de [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista networkIPv6ConfigurationManagementConditions](../api/intune-fencing-networkipv6configurationmanagementcondition-list.md)|coleção [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Lista as propriedades e os relacionamentos dos objetos [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|
|[Obter networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-get.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Leia as propriedades e os relacionamentos do objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|
|[Criar networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-create.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Crie um novo objeto de [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|
|[Excluir networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-delete.md)|Nenhum|Exclui um [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).|
|[Atualizar networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-update.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Atualize as propriedades de um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a condição de gerenciamento. Valor atribuído quando criado gerado pelo sistema. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|nome exclusivo|String|Nome exclusivo para a condição de gerenciamento. Usadas nas expressões de condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|O nome definido admin da condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|String|O administrador definidos descrição da condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi criada. Lado de serviço gerado. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|A hora que da última modificação a condição de gerenciamento. Lado de serviços atualizado. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag da condição de gerenciamento. Lado de serviços atualizado. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|As plataformas aplicáveis para essa condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|ipV6Prefix|String|A sub-rede IPv6 seja conectada. Por exemplo, 2001:db8::/ / 32|
|ipV6Gateway|String|O endereço de gateway IPv6 para. Por exemplo 2001:db8::1|
|ipV6DNSServerList|String collection|Um IPv6 os servidores DNS configurados para o adaptador.|
|dnsSuffixList|String collection|Sufixos DNS válidos para a rede atual. Por exemplo, seattle.contoso.com|

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





