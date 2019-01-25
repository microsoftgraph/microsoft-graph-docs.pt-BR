---
title: tipo de recurso de directoryDefinition
description: Fornece as informações de mecanismo de sincronização sobre um diretório e seus objetos. Este recurso informa ao mecanismo de sincronização, por exemplo, se o diretório tem objetos com o nome de **usuário** e **grupo**, quais atributos são suportados para esses objetos e os tipos para esses atributos. Na ordem para o objeto e o atributo para participar de regras de sincronização e mapeamentos de objeto, ele devem ser definidos como parte da definição do diretório.
localization_priority: Normal
ms.openlocfilehash: 22ba4a7f3b5b5d3154ec6b3f5d42bd6f1b8f09d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508122"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="e1ac4-105">tipo de recurso de directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="e1ac4-105">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1ac4-106">Fornece as informações de mecanismo de sincronização sobre um diretório e seus objetos.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-106">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="e1ac4-107">Este recurso informa ao mecanismo de sincronização, por exemplo, se o diretório tem objetos com o nome de **usuário** e **grupo**, quais atributos são suportados para esses objetos e os tipos para esses atributos.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-107">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="e1ac4-108">Na ordem para o objeto e o atributo para participar de [regras de sincronização](synchronization-synchronizationrule.md) e [mapeamentos de objeto](synchronization-objectmapping.md), ele devem ser definidos como parte da definição do diretório.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-108">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="e1ac4-109">Em geral, o padrão de [esquema de sincronização](synchronization-synchronizationschema.md) fornecido como parte do [modelo de sincronização](synchronization-synchronizationtemplate.md) definirá mais comumente usados objetos e atributos para esse diretório.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-109">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="e1ac4-110">No entanto, se o diretório suporta a adição de atributos personalizados, convém expandir a definição padrão com seus próprios objetos personalizados ou atributos.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-110">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="e1ac4-111">Para obter mais informações, consulte [Configure sincronização com atributos personalizados](synchronization-configure-with-custom-target-attributes.md) e a [sincronização de Configure com atributos de extensão do diretório](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="e1ac4-111">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="e1ac4-112">Definições do diretório são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="e1ac4-112">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e1ac4-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1ac4-113">Properties</span></span>

| <span data-ttu-id="e1ac4-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1ac4-114">Property</span></span>      | <span data-ttu-id="e1ac4-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1ac4-115">Type</span></span>      | <span data-ttu-id="e1ac4-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1ac4-116">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="e1ac4-117">id</span><span class="sxs-lookup"><span data-stu-id="e1ac4-117">id</span></span>           |<span data-ttu-id="e1ac4-118">String</span><span class="sxs-lookup"><span data-stu-id="e1ac4-118">String</span></span>     |<span data-ttu-id="e1ac4-119">Identificador de diretório.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-119">Directory identifier.</span></span> <span data-ttu-id="e1ac4-120">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-120">Not nullable.</span></span>|
|<span data-ttu-id="e1ac4-121">Metadata</span><span class="sxs-lookup"><span data-stu-id="e1ac4-121">metadata</span></span>       |<span data-ttu-id="e1ac4-122">coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="e1ac4-122">metadataEntry collection</span></span>    |<span data-ttu-id="e1ac4-123">Propriedades adicionais de extensão.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-123">Additional extension properties.</span></span> <span data-ttu-id="e1ac4-124">A menos que mencionado explicitamente, valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="e1ac4-125">name</span><span class="sxs-lookup"><span data-stu-id="e1ac4-125">name</span></span>           |<span data-ttu-id="e1ac4-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1ac4-126">String</span></span>     |<span data-ttu-id="e1ac4-127">Nome do diretório.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-127">Name of the directory.</span></span> <span data-ttu-id="e1ac4-128">Deve ser exclusivo dentro do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="e1ac4-128">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="e1ac4-129">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-129">Not nullable.</span></span>|
|<span data-ttu-id="e1ac4-130">Objetos</span><span class="sxs-lookup"><span data-stu-id="e1ac4-130">objects</span></span>        |<span data-ttu-id="e1ac4-131">coleção [objectDefinition](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1ac4-131">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="e1ac4-132">Coleção de objetos compatíveis com o diretório.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-132">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1ac4-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1ac4-133">JSON representation</span></span>

<span data-ttu-id="e1ac4-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1ac4-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="e1ac4-135">Exemplo JSON</span><span class="sxs-lookup"><span data-stu-id="e1ac4-135">JSON Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-directorydefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
