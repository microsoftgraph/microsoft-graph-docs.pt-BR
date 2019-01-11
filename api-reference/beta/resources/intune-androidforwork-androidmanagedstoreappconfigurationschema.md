---
title: tipo de recurso de androidManagedStoreAppConfigurationSchema
description: Esquema que descreve as configurações personalizadas de um aplicativo Android.
localization_priority: Normal
ms.openlocfilehash: 9203d72739da7fa3c4acda0388676ed1c86f924e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880231"
---
# <a name="androidmanagedstoreappconfigurationschema-resource-type"></a>tipo de recurso de androidManagedStoreAppConfigurationSchema

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Esquema que descreve as configurações personalizadas de um aplicativo Android.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista androidManagedStoreAppConfigurationSchemas](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-list.md)|coleção [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Lista as propriedades e os relacionamentos dos objetos [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .|
|[Obter androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-get.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Leia as propriedades e os relacionamentos do objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .|
|[Criar androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-create.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Crie um novo objeto de [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .|
|[Excluir androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-delete.md)|Nenhum|Exclui um [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).|
|[Atualizar androidManagedStoreAppConfigurationSchema](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-update.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Atualize as propriedades de um objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a|
|exampleJson|Binária|A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo|
|schemaItems|coleção [androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)|Conjunto de itens que representa uma opção de configuração nomeada no esquema|

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





