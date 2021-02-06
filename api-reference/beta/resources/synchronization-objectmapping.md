---
title: Tipo de recurso objectMapping
description: Define como um determinado objeto deve ser sincronizado do diretório de origem para o diretório de destino.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 94aa85c198ea67a4c53fc5b56d342188835b0ace
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133169"
---
# <a name="objectmapping-resource-type"></a><span data-ttu-id="cb39f-103">Tipo de recurso objectMapping</span><span class="sxs-lookup"><span data-stu-id="cb39f-103">objectMapping resource type</span></span>

<span data-ttu-id="cb39f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb39f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb39f-105">Define como um determinado objeto deve ser sincronizado do diretório de origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="cb39f-105">Defines how a given object should be synchronized from source directory to target directory.</span></span> <span data-ttu-id="cb39f-106">Em particular, ele define como o objeto no diretório de origem deve ser parecido com um objeto no diretório de destino, quais filtros de scoping (se algum) devem ser usados para decidir se desejamos provisionar um determinado objeto e como os atributos de objeto devem ser transformados indo do diretório de origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="cb39f-106">In particular, it defines how object in source directory should be matched with an object in target directory, what (if any) scoping filters should be used to decide if we want to provision a given object, and how object attributes should be transformed going from source to target directory.</span></span>

<span data-ttu-id="cb39f-107">Os mapeamentos de objetos são a parte principal da regra [de](synchronization-synchronizationrule.md) sincronização e são atualizados como parte do esquema [de sincronização.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="cb39f-107">Object mappings are the main part of the [synchronization rule](synchronization-synchronizationrule.md) and are updated as part of [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cb39f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb39f-108">Properties</span></span>

| <span data-ttu-id="cb39f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb39f-109">Property</span></span>      | <span data-ttu-id="cb39f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb39f-110">Type</span></span>      | <span data-ttu-id="cb39f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb39f-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="cb39f-112">attributeMappings</span><span class="sxs-lookup"><span data-stu-id="cb39f-112">attributeMappings</span></span>  |<span data-ttu-id="cb39f-113">[Coleção attributeMapping](synchronization-attributemapping.md)</span><span class="sxs-lookup"><span data-stu-id="cb39f-113">[attributeMapping](synchronization-attributemapping.md) collection</span></span>    | <span data-ttu-id="cb39f-114">Mapeamentos de atributos definem quais atributos serão mapeados do objeto de origem para o objeto de destino e como eles devem fluir.</span><span class="sxs-lookup"><span data-stu-id="cb39f-114">Attribute mappings define which attributes to map from the source object into the target object and how they should flow.</span></span> <span data-ttu-id="cb39f-115">Várias funções estão disponíveis para dar suporte à transformação dos valores de origem originais.</span><span class="sxs-lookup"><span data-stu-id="cb39f-115">A number of functions are available to support the transformation of the original source values.</span></span>|
|<span data-ttu-id="cb39f-116">enabled</span><span class="sxs-lookup"><span data-stu-id="cb39f-116">enabled</span></span>        |<span data-ttu-id="cb39f-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb39f-117">Boolean</span></span>    |<span data-ttu-id="cb39f-118">Quando `true` , esse mapeamento de objeto será processado durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="cb39f-118">When `true`, this object mapping will be processed during synchronization.</span></span> <span data-ttu-id="cb39f-119">Quando `false` , esse mapeamento de objeto será ignorado.</span><span class="sxs-lookup"><span data-stu-id="cb39f-119">When `false`, this object mapping will be skipped.</span></span>|
|<span data-ttu-id="cb39f-120">flowTypes</span><span class="sxs-lookup"><span data-stu-id="cb39f-120">flowTypes</span></span>      |<span data-ttu-id="cb39f-121">objectFlowTypes</span><span class="sxs-lookup"><span data-stu-id="cb39f-121">objectFlowTypes</span></span>    |<span data-ttu-id="cb39f-122">Quais tipos de fluxo estão habilitados para esse mapeamento de objetos.</span><span class="sxs-lookup"><span data-stu-id="cb39f-122">Which flow types are enabled for this object mapping.</span></span> <span data-ttu-id="cb39f-123">`Add` cria novos objetos no diretório de destino, modifica objetos existentes e `Update` `Delete` desprovisiona os usuários existentes.</span><span class="sxs-lookup"><span data-stu-id="cb39f-123">`Add` creates new objects in the target directory, `Update` modifies existing objects, and `Delete` deprovisions existing users.</span></span> <span data-ttu-id="cb39f-124">O padrão é `Add, Update, Delete` .</span><span class="sxs-lookup"><span data-stu-id="cb39f-124">The default is `Add, Update, Delete`.</span></span> |
|<span data-ttu-id="cb39f-125">metadados</span><span class="sxs-lookup"><span data-stu-id="cb39f-125">metadata</span></span>       |<span data-ttu-id="cb39f-126">Coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="cb39f-126">metadataEntry collection</span></span>    |<span data-ttu-id="cb39f-127">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="cb39f-127">Additional extension properties.</span></span> <span data-ttu-id="cb39f-128">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="cb39f-128">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="cb39f-129">nome</span><span class="sxs-lookup"><span data-stu-id="cb39f-129">name</span></span>           |<span data-ttu-id="cb39f-130">String</span><span class="sxs-lookup"><span data-stu-id="cb39f-130">String</span></span>     |<span data-ttu-id="cb39f-131">Nome amigável do mapeamento de objetos.</span><span class="sxs-lookup"><span data-stu-id="cb39f-131">Human-friendly name of the object mapping.</span></span>|
|<span data-ttu-id="cb39f-132">escopo</span><span class="sxs-lookup"><span data-stu-id="cb39f-132">scope</span></span>          |[<span data-ttu-id="cb39f-133">filter</span><span class="sxs-lookup"><span data-stu-id="cb39f-133">filter</span></span>](synchronization-filter.md)     |<span data-ttu-id="cb39f-134">Define um filtro a ser usado ao decidir se um determinado objeto deve ser provisionado.</span><span class="sxs-lookup"><span data-stu-id="cb39f-134">Defines a filter to be used when deciding whether a given object should be provisioned.</span></span> <span data-ttu-id="cb39f-135">Por exemplo, talvez você queira provisionar apenas usuários localizados nos EUA.</span><span class="sxs-lookup"><span data-stu-id="cb39f-135">For example, you might want to only provision users that are located in the US.</span></span>|
|<span data-ttu-id="cb39f-136">sourceObjectName</span><span class="sxs-lookup"><span data-stu-id="cb39f-136">sourceObjectName</span></span>           |<span data-ttu-id="cb39f-137">String</span><span class="sxs-lookup"><span data-stu-id="cb39f-137">String</span></span>     |<span data-ttu-id="cb39f-138">Nome do objeto no diretório de origem.</span><span class="sxs-lookup"><span data-stu-id="cb39f-138">Name of the object in the source directory.</span></span> <span data-ttu-id="cb39f-139">Deve corresponder ao nome do objeto da definição do [diretório de origem.](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cb39f-139">Must match the object name from the source [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="cb39f-140">targetObjectName</span><span class="sxs-lookup"><span data-stu-id="cb39f-140">targetObjectName</span></span>           |<span data-ttu-id="cb39f-141">String</span><span class="sxs-lookup"><span data-stu-id="cb39f-141">String</span></span>     |<span data-ttu-id="cb39f-142">Nome do objeto no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="cb39f-142">Name of the object in target directory.</span></span> <span data-ttu-id="cb39f-143">Deve corresponder ao nome do objeto da definição do [diretório de destino.](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cb39f-143">Must match the object name from the target [directory definition](synchronization-directorydefinition.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb39f-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb39f-144">JSON representation</span></span>

<span data-ttu-id="cb39f-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb39f-145">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="cb39f-146">Exemplo JSON</span><span class="sxs-lookup"><span data-stu-id="cb39f-146">JSON Example</span></span>

<!-- {
  "blockType": "example",
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
  "suppressions": []
}
-->


