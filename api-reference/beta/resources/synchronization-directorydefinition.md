---
title: tipo de recurso de directoryDefinition
description: Fornece as informações de mecanismo de sincronização sobre um diretório e seus objetos. Este recurso informa ao mecanismo de sincronização, por exemplo, se o diretório tem objetos com o nome de **usuário** e **grupo**, quais atributos são suportados para esses objetos e os tipos para esses atributos. Na ordem para o objeto e o atributo para participar de regras de sincronização e mapeamentos de objeto, ele devem ser definidos como parte da definição do diretório.
ms.openlocfilehash: ddc32237efc18d43da23d815aea00ee01b2650be
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040677"
---
# <a name="directorydefinition-resource-type"></a>tipo de recurso de directoryDefinition

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Fornece as informações de mecanismo de sincronização sobre um diretório e seus objetos. Este recurso informa ao mecanismo de sincronização, por exemplo, se o diretório tem objetos com o nome de **usuário** e **grupo**, quais atributos são suportados para esses objetos e os tipos para esses atributos. Na ordem para o objeto e o atributo para participar de [regras de sincronização](synchronization-synchronizationrule.md) e [mapeamentos de objeto](synchronization-objectmapping.md), ele devem ser definidos como parte da definição do diretório.

Em geral, o padrão de [esquema de sincronização](synchronization-synchronizationschema.md) fornecido como parte do [modelo de sincronização](synchronization-synchronizationtemplate.md) definirá mais comumente usados objetos e atributos para esse diretório. No entanto, se o diretório suporta a adição de atributos personalizados, convém expandir a definição padrão com seus próprios objetos personalizados ou atributos. Para obter mais informações, consulte [Configure sincronização com atributos personalizados](synchronization-configure-with-custom-target-attributes.md) e a [sincronização de Configure com atributos de extensão do diretório](synchronization-configure-with-directory-extension-attributes.md).

Definições do diretório são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|id           |String     |Identificador de diretório. Não anulável.|
|metadados       |coleção metadataEntry    |Propriedades adicionais de extensão. A menos que mencionado explicitamente, valores de metadados não devem ser alterados.|
|name           |String     |Nome do diretório. Deve ser exclusivo dentro do [esquema de sincronização](synchronization-synchronizationschema.md). Não anulável.|
|objetos        |coleção [objectDefinition](synchronization-objectdefinition.md)    |Coleção de objetos compatíveis com o diretório.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "id": "String",
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}]
}

```

## <a name="json-example"></a>Exemplo JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
    "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
    "name": "salesforce.com",
    "objects": [
        {
            "attributes": [
                {
                    "anchor": true,
                    "name": "Id",
                    "type": "String"
                },
                {
                    "name": "IsActive",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "mutability": "ReadWrite",
                    "name": "Alias",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "CompanyName",
                    "type": "String"
                },
                {
                    "name": "CommunityNickname",
                    "type": "String"
                },
                {
                    "name": "Email",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "EmailEncodingKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LanguageLocaleKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "FirstName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LastName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LocaleSidKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "metadata": [
                        {
                            "key": "LinkTypeName",
                            "value": "PermissionSetAssignment"
                        },
                        {
                            "key": "LinkPropertyNames",
                            "value": "[\"PermissionSetId\"]"
                        }
                    ],
                    "name": "PermissionSets",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "PermissionSet"
                        }
                    ],
                    "type": "Reference"
                },
                {
                    "name": "ProfileId",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "ProfileName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "TimeZoneSidKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "Username",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "UserPermissionsCallCenterAutoLogin",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "name": "UserPermissionsMarketingUser",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "name": "Street",
                    "type": "String"
                },
                {
                    "name": "City",
                    "type": "String"
                },
                {
                    "name": "Division",
                    "type": "String"
                },
                {
                    "name": "EmployeeNumber",
                    "type": "String"
                },
                {
                    "name": "State",
                    "type": "String"
                },
                {
                    "name": "PostalCode",
                    "type": "String"
                },
                {
                    "name": "Country",
                    "type": "String"
                },
                {
                    "name": "Department",
                    "type": "String"
                },
                {
                    "name": "MobilePhone",
                    "type": "String"
                },
                {
                    "name": "Phone",
                    "type": "String"
                },
                {
                    "name": "Title",
                    "type": "String"
                },
                {
                    "name": "FederationIdentifier",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "ManagerId",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "User"
                        }
                    ],
                    "type": "Reference"
                },
                {
                    "name": "UserRoleId",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "UserRole"
                        }
                    ],
                    "type": "Reference"
                }
            ],
            "metadata": [
                {
                    "key": "IsSoftDeletionSupported",
                    "value": "false"
                },
                {
                    "key": "ConnectorDataStorageRequired",
                    "value": "false"
                },
                {
                    "key": "IsSynchronizeAllSupported",
                    "value": "false"
                }
            ],
            "name": "User"
        }
    ],
    "metadata": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->