---
title: Tipo de recurso targetedManagedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para todos os usuários do grupo de segurança visado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5671cf59c9fb45d12c6e31bccfa929d5e800b0050b9c660474a611ca295bc09c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230540"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a>Tipo de recurso targetedManagedAppConfiguration

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para todos os usuários do grupo de segurança visado


Herda de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar targetedManagedAppConfigurations](../api/intune-mam-targetedmanagedappconfiguration-list.md)|Coleção [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Listar propriedades e relações dos objetos [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).|
|[Obter targetedManagedAppConfiguration](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Ler propriedades e relações do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).|
|[Criar targetedManagedAppConfiguration](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Cria um novo objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).|
|[Excluir targetedManagedAppConfiguration](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|Nenhum|Excluir um [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).|
|[Atualizar targetedManagedAppConfiguration](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).|
|[Ação assign](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|Nenhuma|Ainda não documentado|
|[Ação targetApps](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|Cadeia de caracteres|A descrição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|Versão da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|customSettings|Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)|Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)|
|deployedAppCount|Int32|Contagem de aplicativos em que a política atual é implantada.|
|isAssigned|Boolean|Indica se a política foi implantada a grupos de inclusão ou não.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|apps|Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Lista de aplicativos em que a política é implantada.|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Propriedade de navegação para o resumo de implantação da configuração.|
|assignments|Conjunto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Propriedades de navegação para lista de grupos de inclusão e exclusão às quais a política é implantada.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "isAssigned": true
}
```




