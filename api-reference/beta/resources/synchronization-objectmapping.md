---
title: tipo de recurso objectMapping
description: Define como um determinado objeto deve ser sincronizado do diretório de origem para o diretório de destino. Em particular, define como o objeto no diretório de origem deve corresponder a um objeto no diretório de destino, quais filtros de escopo (se houver) devem ser usados para decidir se queremos provisionar um determinado objeto e como os atributos do objeto devem ser transformados origem para o diretório de destino.
localization_priority: Normal
ms.openlocfilehash: 274d401c28abc25d904c259b00a673f3c0a53888
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581749"
---
# <a name="objectmapping-resource-type"></a><span data-ttu-id="c06b6-104">tipo de recurso objectMapping</span><span class="sxs-lookup"><span data-stu-id="c06b6-104">objectMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c06b6-105">Define como um determinado objeto deve ser sincronizado do diretório de origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="c06b6-105">Defines how a given object should be synchronized from source directory to target directory.</span></span> <span data-ttu-id="c06b6-106">Em particular, define como o objeto no diretório de origem deve corresponder a um objeto no diretório de destino, quais filtros de escopo (se houver) devem ser usados para decidir se queremos provisionar um determinado objeto e como os atributos do objeto devem ser transformados origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="c06b6-106">In particular, it defines how object in source directory should be matched with an object in target directory, what (if any) scoping filters should be used to decide if we want to provision a given object, and how object attributes should be transformed going from source to target directory.</span></span>

<span data-ttu-id="c06b6-107">Os mapeamentos de objetos são a parte principal da [regra de sincronização](synchronization-synchronizationrule.md) e são atualizados como parte do esquema de [sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="c06b6-107">Object mappings are the main part of the [synchronization rule](synchronization-synchronizationrule.md) and are updated as part of [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c06b6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c06b6-108">Properties</span></span>

| <span data-ttu-id="c06b6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c06b6-109">Property</span></span>      | <span data-ttu-id="c06b6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c06b6-110">Type</span></span>      | <span data-ttu-id="c06b6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c06b6-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="c06b6-112">attributeMappings</span><span class="sxs-lookup"><span data-stu-id="c06b6-112">attributeMappings</span></span>  |<span data-ttu-id="c06b6-113">coleção [attributeMapping](synchronization-attributemapping.md)</span><span class="sxs-lookup"><span data-stu-id="c06b6-113">[attributeMapping](synchronization-attributemapping.md) collection</span></span>    | <span data-ttu-id="c06b6-114">Os mapeamentos de atributo definem quais atributos devem ser mapeados do objeto de origem para o objeto de destino e como eles devem fluir.</span><span class="sxs-lookup"><span data-stu-id="c06b6-114">Attribute mappings define which attributes to map from the source object into the target object and how they should flow.</span></span> <span data-ttu-id="c06b6-115">Várias funções estão disponíveis para dar suporte à transformação dos valores de origem originais.</span><span class="sxs-lookup"><span data-stu-id="c06b6-115">A number of functions are available to support the transformation of the original source values.</span></span>|
|<span data-ttu-id="c06b6-116">enabled</span><span class="sxs-lookup"><span data-stu-id="c06b6-116">enabled</span></span>        |<span data-ttu-id="c06b6-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c06b6-117">Boolean</span></span>    |<span data-ttu-id="c06b6-118">Quando `true`, esse mapeamento de objeto será processado durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="c06b6-118">When `true`, this object mapping will be processed during synchronization.</span></span> <span data-ttu-id="c06b6-119">Quando `false`, esse mapeamento de objeto será ignorado.</span><span class="sxs-lookup"><span data-stu-id="c06b6-119">When `false`, this object mapping will be skipped.</span></span>|
|<span data-ttu-id="c06b6-120">flowTypes</span><span class="sxs-lookup"><span data-stu-id="c06b6-120">flowTypes</span></span>      |<span data-ttu-id="c06b6-121">objectFlowtype</span><span class="sxs-lookup"><span data-stu-id="c06b6-121">objectFlowType</span></span>    |<span data-ttu-id="c06b6-122">Quais tipos de fluxo estão habilitados para este mapeamento de objeto.</span><span class="sxs-lookup"><span data-stu-id="c06b6-122">Which flow types are enabled for this object mapping.</span></span> <span data-ttu-id="c06b6-123">`Add`cria novos objetos no diretório de destino, `Update` modifica objetos existentes e `Delete` desprovisiona usuários existentes.</span><span class="sxs-lookup"><span data-stu-id="c06b6-123">`Add` creates new objects in the target directory, `Update` modifies existing objects, and `Delete` deprovisions existing users.</span></span> <span data-ttu-id="c06b6-124">O padrão é `Add, Update, Delete`.</span><span class="sxs-lookup"><span data-stu-id="c06b6-124">The default is `Add, Update, Delete`.</span></span> |
|<span data-ttu-id="c06b6-125">los</span><span class="sxs-lookup"><span data-stu-id="c06b6-125">metadata</span></span>       |<span data-ttu-id="c06b6-126">coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="c06b6-126">metadataEntry collection</span></span>    |<span data-ttu-id="c06b6-127">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="c06b6-127">Additional extension properties.</span></span> <span data-ttu-id="c06b6-128">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="c06b6-128">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="c06b6-129">name</span><span class="sxs-lookup"><span data-stu-id="c06b6-129">name</span></span>           |<span data-ttu-id="c06b6-130">String</span><span class="sxs-lookup"><span data-stu-id="c06b6-130">String</span></span>     |<span data-ttu-id="c06b6-131">Nome amigável do mapeamento do objeto.</span><span class="sxs-lookup"><span data-stu-id="c06b6-131">Human-friendly name of the object mapping.</span></span>|
|<span data-ttu-id="c06b6-132">escopo</span><span class="sxs-lookup"><span data-stu-id="c06b6-132">scope</span></span>          |[<span data-ttu-id="c06b6-133">filter</span><span class="sxs-lookup"><span data-stu-id="c06b6-133">filter</span></span>](synchronization-filter.md)     |<span data-ttu-id="c06b6-134">Define um filtro a ser usado ao decidir se um determinado objeto deve ser provisionado.</span><span class="sxs-lookup"><span data-stu-id="c06b6-134">Defines a filter to be used when deciding whether a given object should be provisioned.</span></span> <span data-ttu-id="c06b6-135">Por exemplo, você pode querer provisionar apenas usuários que estão localizados nos EUA.</span><span class="sxs-lookup"><span data-stu-id="c06b6-135">For example, you might want to only provision users that are located in the US.</span></span>|
|<span data-ttu-id="c06b6-136">sourceObjectName</span><span class="sxs-lookup"><span data-stu-id="c06b6-136">sourceObjectName</span></span>           |<span data-ttu-id="c06b6-137">String</span><span class="sxs-lookup"><span data-stu-id="c06b6-137">String</span></span>     |<span data-ttu-id="c06b6-138">Nome do objeto no diretório de origem.</span><span class="sxs-lookup"><span data-stu-id="c06b6-138">Name of the object in the source directory.</span></span> <span data-ttu-id="c06b6-139">Deve corresponder ao nome do objeto da [definição do diretório](synchronization-directorydefinition.md)de origem.</span><span class="sxs-lookup"><span data-stu-id="c06b6-139">Must match the object name from the source [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="c06b6-140">targetObjectName</span><span class="sxs-lookup"><span data-stu-id="c06b6-140">targetObjectName</span></span>           |<span data-ttu-id="c06b6-141">String</span><span class="sxs-lookup"><span data-stu-id="c06b6-141">String</span></span>     |<span data-ttu-id="c06b6-142">Nome do objeto no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="c06b6-142">Name of the object in target directory.</span></span> <span data-ttu-id="c06b6-143">Deve corresponder ao nome do objeto da [definição do diretório](synchronization-directorydefinition.md)de destino.</span><span class="sxs-lookup"><span data-stu-id="c06b6-143">Must match the object name from the target [directory definition](synchronization-directorydefinition.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c06b6-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c06b6-144">JSON representation</span></span>

<span data-ttu-id="c06b6-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c06b6-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectMapping"
}-->

```json
{
  "attributeMappings": [{"@odata.type": "microsoft.graph.attributeMapping"}],
  "enabled": true,
  "flowTypes": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "name": "String",
  "scope": {"@odata.type": "microsoft.graph.filter"},
  "sourceObjectName": "String",
  "targetObjectName": "String"
}
```

## <a name="json-example"></a><span data-ttu-id="c06b6-146">Exemplo de JSON</span><span class="sxs-lookup"><span data-stu-id="c06b6-146">JSON Example</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectMapping"
}-->

```json
{
    "attributeMappings": [
        {
            "defaultValue": "True",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Not([IsSoftDeleted])",
                "name": "Not",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[IsSoftDeleted]",
                            "name": "IsSoftDeleted",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "IsActive"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Mid([userPrincipalName], 1, 8)",
                "name": "Mid",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[userPrincipalName]",
                            "name": "userPrincipalName",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    },
                    {
                        "key": "start",
                        "value": {
                            "expression": "\"1\"",
                            "name": "1",
                            "parameters": [],
                            "type": "Constant"
                        }
                    },
                    {
                        "key": "length",
                        "value": {
                            "expression": "\"8\"",
                            "name": "8",
                            "parameters": [],
                            "type": "Constant"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "Alias"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[mail]",
                "name": "mail",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "Email"
        },
        {
            "defaultValue": "ISO-8859-1",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "EmailEncodingKey"
        },
        {
            "defaultValue": "en_US",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "LanguageLocaleKey"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[givenName]",
                "name": "givenName",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "FirstName"
        },
        {
            "defaultValue": ".",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[surname]",
                "name": "surname",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "LastName"
        },
        {
            "defaultValue": "en_US",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Replace([preferredLanguage], \"-\", , , \"_\", , )",
                "name": "Replace",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[preferredLanguage]",
                            "name": "preferredLanguage",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    },
                    {
                        "key": "Find",
                        "value": {
                            "expression": "\"-\"",
                            "name": "-",
                            "parameters": [],
                            "type": "Constant"
                        }
                    },
                    {
                        "key": "Replacement",
                        "value": {
                            "expression": "\"_\"",
                            "name": "_",
                            "parameters": [],
                            "type": "Constant"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "LocaleSidKey"
        },
        {
            "defaultValue": "Chatter Free User",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "SingleAppRoleAssignment([appRoleAssignments])",
                "name": "SingleAppRoleAssignment",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[appRoleAssignments]",
                            "name": "appRoleAssignments",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "ProfileName"
        },
        {
            "defaultValue": "America/Los_Angeles",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "TimeZoneSidKey"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 1,
            "source": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "Username"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsCallCenterAutoLogin"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsMarketingUser"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsOfflineUser"
        }
    ],
    "enabled": true,
    "flowTypes": "Add, Update, Delete",
    "metadata": [
        {
            "key": "IsCustomerDefined",
            "value": "false"
        },
        {
            "key": "DisableMonitoringForChanges",
            "value": "false"
        },
        {
            "key": "Disposition",
            "value": "\"Normal\""
        },
        {
            "key": "ExcludeFromReporting",
            "value": "false"
        },
        {
            "key": "EscrowBehavior",
            "value": "\"Default\""
        },
        {
            "key": "Unsynchronized",
            "value": "false"
        }
    ],
    "name": "Synchronize Azure Active Directory Users to salesforce.com",
    "scope": null,
    "sourceObjectName": "User",
    "targetObjectName": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-objectmapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
