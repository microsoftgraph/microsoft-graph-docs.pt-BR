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
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="ba208-105">tipo de recurso de directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="ba208-105">directoryDefinition resource type</span></span>

> <span data-ttu-id="ba208-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ba208-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba208-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ba208-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba208-108">Fornece as informações de mecanismo de sincronização sobre um diretório e seus objetos.</span><span class="sxs-lookup"><span data-stu-id="ba208-108">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="ba208-109">Este recurso informa ao mecanismo de sincronização, por exemplo, se o diretório tem objetos com o nome de **usuário** e **grupo**, quais atributos são suportados para esses objetos e os tipos para esses atributos.</span><span class="sxs-lookup"><span data-stu-id="ba208-109">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="ba208-110">Na ordem para o objeto e o atributo para participar de [regras de sincronização](synchronization-synchronizationrule.md) e [mapeamentos de objeto](synchronization-objectmapping.md), ele devem ser definidos como parte da definição do diretório.</span><span class="sxs-lookup"><span data-stu-id="ba208-110">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="ba208-111">Em geral, o padrão de [esquema de sincronização](synchronization-synchronizationschema.md) fornecido como parte do [modelo de sincronização](synchronization-synchronizationtemplate.md) definirá mais comumente usados objetos e atributos para esse diretório.</span><span class="sxs-lookup"><span data-stu-id="ba208-111">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="ba208-112">No entanto, se o diretório suporta a adição de atributos personalizados, convém expandir a definição padrão com seus próprios objetos personalizados ou atributos.</span><span class="sxs-lookup"><span data-stu-id="ba208-112">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="ba208-113">Para obter mais informações, consulte [Configure sincronização com atributos personalizados](synchronization-configure-with-custom-target-attributes.md) e a [sincronização de Configure com atributos de extensão do diretório](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="ba208-113">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="ba208-114">Definições do diretório são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="ba208-114">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ba208-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba208-115">Properties</span></span>

| <span data-ttu-id="ba208-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba208-116">Property</span></span>      | <span data-ttu-id="ba208-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba208-117">Type</span></span>      | <span data-ttu-id="ba208-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba208-118">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="ba208-119">id</span><span class="sxs-lookup"><span data-stu-id="ba208-119">id</span></span>           |<span data-ttu-id="ba208-120">String</span><span class="sxs-lookup"><span data-stu-id="ba208-120">String</span></span>     |<span data-ttu-id="ba208-121">Identificador de diretório.</span><span class="sxs-lookup"><span data-stu-id="ba208-121">Directory identifier.</span></span> <span data-ttu-id="ba208-122">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ba208-122">Not nullable.</span></span>|
|<span data-ttu-id="ba208-123">metadados</span><span class="sxs-lookup"><span data-stu-id="ba208-123">metadata</span></span>       |<span data-ttu-id="ba208-124">coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="ba208-124">metadataEntry collection</span></span>    |<span data-ttu-id="ba208-125">Propriedades adicionais de extensão.</span><span class="sxs-lookup"><span data-stu-id="ba208-125">Additional extension properties.</span></span> <span data-ttu-id="ba208-126">A menos que mencionado explicitamente, valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="ba208-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="ba208-127">name</span><span class="sxs-lookup"><span data-stu-id="ba208-127">name</span></span>           |<span data-ttu-id="ba208-128">String</span><span class="sxs-lookup"><span data-stu-id="ba208-128">String</span></span>     |<span data-ttu-id="ba208-129">Nome do diretório.</span><span class="sxs-lookup"><span data-stu-id="ba208-129">Name of the directory.</span></span> <span data-ttu-id="ba208-130">Deve ser exclusivo dentro do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="ba208-130">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="ba208-131">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ba208-131">Not nullable.</span></span>|
|<span data-ttu-id="ba208-132">objetos</span><span class="sxs-lookup"><span data-stu-id="ba208-132">objects</span></span>        |<span data-ttu-id="ba208-133">coleção [objectDefinition](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ba208-133">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="ba208-134">Coleção de objetos compatíveis com o diretório.</span><span class="sxs-lookup"><span data-stu-id="ba208-134">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba208-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba208-135">JSON representation</span></span>

<span data-ttu-id="ba208-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba208-136">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="ba208-137">Exemplo JSON</span><span class="sxs-lookup"><span data-stu-id="ba208-137">JSON Example</span></span>

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