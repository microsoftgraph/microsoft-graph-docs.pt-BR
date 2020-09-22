---
title: tipo de recurso ObjectDefinition
description: Descreve um objeto e seus atributos.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0048d11a8241e8a81bf223f337493e37aebaceda
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016013"
---
# <a name="objectdefinition-resource-type"></a><span data-ttu-id="4c19b-103">tipo de recurso ObjectDefinition</span><span class="sxs-lookup"><span data-stu-id="4c19b-103">objectDefinition resource type</span></span>

<span data-ttu-id="4c19b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c19b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c19b-105">Descreve um objeto e seus atributos.</span><span class="sxs-lookup"><span data-stu-id="4c19b-105">Describes an object and its attributes.</span></span> <span data-ttu-id="4c19b-106">As definições de objeto fazem parte do [directoryDefinition](synchronization-directorydefinition.md), que é atualizado como parte do [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="4c19b-106">Object definitions are part of [directoryDefinition](synchronization-directorydefinition.md), which is updated as part of [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4c19b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c19b-107">Properties</span></span>

| <span data-ttu-id="4c19b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c19b-108">Property</span></span>      | <span data-ttu-id="4c19b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c19b-109">Type</span></span>      | <span data-ttu-id="4c19b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c19b-110">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="4c19b-111">attributes</span><span class="sxs-lookup"><span data-stu-id="4c19b-111">attributes</span></span>     |<span data-ttu-id="4c19b-112">coleção [attributeDefinition](synchronization-attributedefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4c19b-112">[attributeDefinition](synchronization-attributedefinition.md) collection</span></span>    | <span data-ttu-id="4c19b-113">Define os atributos do objeto.</span><span class="sxs-lookup"><span data-stu-id="4c19b-113">Defines attributes of the object.</span></span> |
|<span data-ttu-id="4c19b-114">los</span><span class="sxs-lookup"><span data-stu-id="4c19b-114">metadata</span></span>       |<span data-ttu-id="4c19b-115">coleção [metadataEntry](synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="4c19b-115">[metadataEntry](synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="4c19b-116">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="4c19b-116">Additional extension properties.</span></span> <span data-ttu-id="4c19b-117">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="4c19b-117">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="4c19b-118">nome</span><span class="sxs-lookup"><span data-stu-id="4c19b-118">name</span></span>           |<span data-ttu-id="4c19b-119">String</span><span class="sxs-lookup"><span data-stu-id="4c19b-119">String</span></span>     |<span data-ttu-id="4c19b-120">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="4c19b-120">Name of the object.</span></span> <span data-ttu-id="4c19b-121">Deve ser exclusivo dentro de uma definição de diretório.</span><span class="sxs-lookup"><span data-stu-id="4c19b-121">Must be unique within a directory definition.</span></span> <span data-ttu-id="4c19b-122">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="4c19b-122">Not nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c19b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c19b-123">JSON representation</span></span>

<span data-ttu-id="4c19b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c19b-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectDefinition"
}-->

```json
{
  "attributes": [{"@odata.type": "microsoft.graph.attributeDefinition"}],
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "name": "String"
}
```

## <a name="json-example"></a><span data-ttu-id="4c19b-125">Exemplo de JSON</span><span class="sxs-lookup"><span data-stu-id="4c19b-125">JSON Example</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectDefinition"
}-->

```json
{
    "attributes": [
        {
            "anchor": true,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "objectId",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "IsSoftDeleted",
            "required": true,
            "referencedObjects": [],
            "type": "Boolean"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "accountEnabled",
            "required": true,
            "referencedObjects": [],
            "type": "Boolean"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "streetAddress",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "city",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "state",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "postalCode",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "country",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "companyName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "department",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "dirSyncEnabled",
            "required": false,
            "referencedObjects": [],
            "type": "Boolean"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "displayName",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "extensionAttribute1",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "facsimileTelephoneNumber",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "givenName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "jobTitle",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "mail",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "mailNickname",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "manager",
            "required": false,
            "referencedObjects": [
                {
                    "referencedObjectName": "User",
                    "referencedProperty": null
                }
            ],
            "type": "Reference"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "mobile",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "onPremisesSecurityIdentifier",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "originalUserPrincipalName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "passwordProfile.password",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "physicalDeliveryOfficeName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "preferredLanguage",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": true,
            "mutability": "ReadWrite",
            "name": "proxyAddresses",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "surname",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "telephoneNumber",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "userPrincipalName",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        }
    ],
    "metadata": [
        {
            "key": "IsSoftDeletionSupported",
            "value": "true"
        },
        {
            "key": "ConnectorDataStorageRequired",
            "value": "true"
        },
        {
            "key": "IsSynchronizeAllSupported",
            "value": "true"
        },
        {
            "key": "PropertyNameAccountEnabled",
            "value": "accountEnabled"
        },
        {
            "key": "PropertyNameSoftDeleted",
            "value": "IsSoftDeleted"
        }
    ],
    "name": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


