---
title: tipo de recurso androidManagedStoreAppConfigurationSchema
description: Esquema que descreve as configurações personalizadas de um aplicativo Android.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5445f0bec409f823c1c4fad1586448a76d11180b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030540"
---
# <a name="androidmanagedstoreappconfigurationschema-resource-type"></a>tipo de recurso androidManagedStoreAppConfigurationSchema

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Esquema que descreve as configurações personalizadas de um aplicativo Android.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidManagedStoreAppConfigurationSchemas](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-list.md)|[coleção androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Listar propriedades e relações dos objetos [androidManagedStoreAppConfigurationSchema.](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|
|[Obter androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-get.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Leia propriedades e relações do [objeto androidManagedStoreAppConfigurationSchema.](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|
|[Criar androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-create.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Crie um novo [objeto androidManagedStoreAppConfigurationSchema.](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|
|[Excluir androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-delete.md)|Nenhum|Exclui um [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).|
|[Atualizar androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-update.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Atualize as propriedades de [um objeto androidManagedStoreAppConfigurationSchema.](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a|
|exampleJson|Binária|A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo|
|schemaItems|[coleção androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)|Coleção de itens que representam uma opção de configuração nomeada no esquema. Ele contém apenas a configuração de nível raiz.|
|nestedSchemaItems|[coleção androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)|Coleção de itens que representam uma opção de configuração nomeada no esquema. Ele contém uma lista simples de todas as configurações.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 1024,
      "parentIndex": 1024,
      "schemaItemKey": "String",
      "displayName": "String",
      "description": "String",
      "defaultBoolValue": true,
      "defaultIntValue": 1024,
      "defaultStringValue": "String",
      "defaultStringArrayValue": [
        "String"
      ],
      "dataType": "String",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "String",
          "value": "String"
        }
      ]
    }
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 1024,
      "parentIndex": 1024,
      "schemaItemKey": "String",
      "displayName": "String",
      "description": "String",
      "defaultBoolValue": true,
      "defaultIntValue": 1024,
      "defaultStringValue": "String",
      "defaultStringArrayValue": [
        "String"
      ],
      "dataType": "String",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "String",
          "value": "String"
        }
      ]
    }
  ]
}
```



