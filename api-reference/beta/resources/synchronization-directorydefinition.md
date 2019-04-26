---
title: tipo de recurso directoryDefinition
description: Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos. Esse recurso instrui o mecanismo de sincronização, por exemplo, que o diretório tem objetos chamados **usuário** e **grupo**, quais atributos são compatíveis com esses objetos e os tipos desses atributos. Para que o objeto e o atributo participem das regras de sincronização e dos mapeamentos de objetos, eles devem ser definidos como parte da definição de diretório.
localization_priority: Normal
ms.openlocfilehash: 8e622edef39eec5476015ef5e22c5fe9697e0daa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342885"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="10247-105">tipo de recurso directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="10247-105">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10247-106">Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos.</span><span class="sxs-lookup"><span data-stu-id="10247-106">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="10247-107">Esse recurso instrui o mecanismo de sincronização, por exemplo, que o diretório tem objetos chamados **usuário** e **grupo**, quais atributos são compatíveis com esses objetos e os tipos desses atributos.</span><span class="sxs-lookup"><span data-stu-id="10247-107">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="10247-108">Para que o objeto e o atributo participem das [regras de sincronização](synchronization-synchronizationrule.md) e dos mapeamentos de [objetos](synchronization-objectmapping.md), eles devem ser definidos como parte da definição de diretório.</span><span class="sxs-lookup"><span data-stu-id="10247-108">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="10247-109">Em geral, o [esquema de sincronização](synchronization-synchronizationschema.md) padrão fornecido como parte do [modelo de sincronização](synchronization-synchronizationtemplate.md) definirá os objetos e atributos usados com mais frequência para esse diretório.</span><span class="sxs-lookup"><span data-stu-id="10247-109">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="10247-110">No enTanto, se o diretório oferecer suporte à adição de atributos personalizados, convém expandir a definição padrão com seus próprios objetos ou atributos personalizados.</span><span class="sxs-lookup"><span data-stu-id="10247-110">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="10247-111">Para obter mais informações, consulte [Configurar a sincronização com atributos personalizados](synchronization-configure-with-custom-target-attributes.md) e [Configurar a sincronização com atributos de extensão de diretório](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="10247-111">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="10247-112">As definições de diretório são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="10247-112">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="10247-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10247-113">Properties</span></span>

| <span data-ttu-id="10247-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10247-114">Property</span></span>      | <span data-ttu-id="10247-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="10247-115">Type</span></span>      | <span data-ttu-id="10247-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="10247-116">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="10247-117">id</span><span class="sxs-lookup"><span data-stu-id="10247-117">id</span></span>           |<span data-ttu-id="10247-118">String</span><span class="sxs-lookup"><span data-stu-id="10247-118">String</span></span>     |<span data-ttu-id="10247-119">Identificador de diretório.</span><span class="sxs-lookup"><span data-stu-id="10247-119">Directory identifier.</span></span> <span data-ttu-id="10247-120">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="10247-120">Not nullable.</span></span>|
|<span data-ttu-id="10247-121">los</span><span class="sxs-lookup"><span data-stu-id="10247-121">metadata</span></span>       |<span data-ttu-id="10247-122">coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="10247-122">metadataEntry collection</span></span>    |<span data-ttu-id="10247-123">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="10247-123">Additional extension properties.</span></span> <span data-ttu-id="10247-124">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="10247-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="10247-125">name</span><span class="sxs-lookup"><span data-stu-id="10247-125">name</span></span>           |<span data-ttu-id="10247-126">String</span><span class="sxs-lookup"><span data-stu-id="10247-126">String</span></span>     |<span data-ttu-id="10247-127">Nome do diretório.</span><span class="sxs-lookup"><span data-stu-id="10247-127">Name of the directory.</span></span> <span data-ttu-id="10247-128">Deve ser exclusivo no [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="10247-128">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="10247-129">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="10247-129">Not nullable.</span></span>|
|<span data-ttu-id="10247-130">objectos</span><span class="sxs-lookup"><span data-stu-id="10247-130">objects</span></span>        |<span data-ttu-id="10247-131">[](synchronization-objectdefinition.md) coleção ObjectDefinition</span><span class="sxs-lookup"><span data-stu-id="10247-131">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="10247-132">Conjunto de objetos suportados pelo diretório.</span><span class="sxs-lookup"><span data-stu-id="10247-132">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10247-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10247-133">JSON representation</span></span>

<span data-ttu-id="10247-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10247-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="10247-135">Exemplo de JSON</span><span class="sxs-lookup"><span data-stu-id="10247-135">JSON Example</span></span>

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
  "suppressions": []
}
-->
