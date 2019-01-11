---
title: tipo de recurso de objectMapping
description: Define como um determinado objeto deve ser sincronizado do diretório de origem para o diretório de destino. Especificamente, ele define como o objeto no diretório de origem deve ser correspondido com um objeto no diretório de destino, o que (se houver) filtros de escopo deve ser usado para decidir se queremos provisionar um determinado objeto e como os atributos de objetos devem ser transformadas contínuas de fonte para o diretório de destino.
localization_priority: Normal
ms.openlocfilehash: 21e996b72be7df93c86f9e5f78a0033c9203cd2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851747"
---
# <a name="objectmapping-resource-type"></a><span data-ttu-id="6b05a-104">tipo de recurso de objectMapping</span><span class="sxs-lookup"><span data-stu-id="6b05a-104">objectMapping resource type</span></span>

> <span data-ttu-id="6b05a-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6b05a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b05a-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6b05a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b05a-107">Define como um determinado objeto deve ser sincronizado do diretório de origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="6b05a-107">Defines how a given object should be synchronized from source directory to target directory.</span></span> <span data-ttu-id="6b05a-108">Especificamente, ele define como o objeto no diretório de origem deve ser correspondido com um objeto no diretório de destino, o que (se houver) filtros de escopo deve ser usado para decidir se queremos provisionar um determinado objeto e como os atributos de objetos devem ser transformadas contínuas de fonte para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="6b05a-108">In particular, it defines how object in source directory should be matched with an object in target directory, what (if any) scoping filters should be used to decide if we want to provision a given object, and how object attributes should be transformed going from source to target directory.</span></span>

<span data-ttu-id="6b05a-109">Mapeamentos de objeto são a parte principal da [regra de sincronização](synchronization-synchronizationrule.md) e serão atualizados como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="6b05a-109">Object mappings are the main part of the [synchronization rule](synchronization-synchronizationrule.md) and are updated as part of [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6b05a-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b05a-110">Properties</span></span>

| <span data-ttu-id="6b05a-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b05a-111">Property</span></span>      | <span data-ttu-id="6b05a-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b05a-112">Type</span></span>      | <span data-ttu-id="6b05a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b05a-113">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="6b05a-114">attributeMappings</span><span class="sxs-lookup"><span data-stu-id="6b05a-114">attributeMappings</span></span>  |<span data-ttu-id="6b05a-115">coleção [attributeMapping](synchronization-attributemapping.md)</span><span class="sxs-lookup"><span data-stu-id="6b05a-115">[attributeMapping](synchronization-attributemapping.md) collection</span></span>    | <span data-ttu-id="6b05a-116">Mapeamentos de atributos definem os atributos a serem mapeadas do objeto de origem para o objeto de destino e como eles deverão fluir.</span><span class="sxs-lookup"><span data-stu-id="6b05a-116">Attribute mappings define which attributes to map from the source object into the target object and how they should flow.</span></span> <span data-ttu-id="6b05a-117">Um número de funções está disponível para dar suporte a transformação dos valores de fonte original.</span><span class="sxs-lookup"><span data-stu-id="6b05a-117">A number of functions are available to support the transformation of the original source values.</span></span>|
|<span data-ttu-id="6b05a-118">enabled</span><span class="sxs-lookup"><span data-stu-id="6b05a-118">enabled</span></span>        |<span data-ttu-id="6b05a-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="6b05a-119">Boolean</span></span>    |<span data-ttu-id="6b05a-120">Quando `true`, esse mapeamento do objeto será processado durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="6b05a-120">When `true`, this object mapping will be processed during synchronization.</span></span> <span data-ttu-id="6b05a-121">Quando `false`, esse mapeamento do objeto será ignorado.</span><span class="sxs-lookup"><span data-stu-id="6b05a-121">When `false`, this object mapping will be skipped.</span></span>|
|<span data-ttu-id="6b05a-122">flowTypes</span><span class="sxs-lookup"><span data-stu-id="6b05a-122">flowTypes</span></span>      |<span data-ttu-id="6b05a-123">objectFlowType</span><span class="sxs-lookup"><span data-stu-id="6b05a-123">objectFlowType</span></span>    |<span data-ttu-id="6b05a-124">Quais tipos de fluxo estão habilitados para esse mapeamento de objeto.</span><span class="sxs-lookup"><span data-stu-id="6b05a-124">Which flow types are enabled for this object mapping.</span></span> <span data-ttu-id="6b05a-125">`Add`cria novos objetos no diretório de destino, `Update` modifica objetos existentes, e `Delete` deprovisions usuários existentes.</span><span class="sxs-lookup"><span data-stu-id="6b05a-125">`Add` creates new objects in the target directory, `Update` modifies existing objects, and `Delete` deprovisions existing users.</span></span> <span data-ttu-id="6b05a-126">O padrão é `Add, Update, Delete`.</span><span class="sxs-lookup"><span data-stu-id="6b05a-126">The default is `Add, Update, Delete`.</span></span> |
|<span data-ttu-id="6b05a-127">metadados</span><span class="sxs-lookup"><span data-stu-id="6b05a-127">metadata</span></span>       |<span data-ttu-id="6b05a-128">coleção metadataEntry</span><span class="sxs-lookup"><span data-stu-id="6b05a-128">metadataEntry collection</span></span>    |<span data-ttu-id="6b05a-129">Propriedades adicionais de extensão.</span><span class="sxs-lookup"><span data-stu-id="6b05a-129">Additional extension properties.</span></span> <span data-ttu-id="6b05a-130">A menos que mencionado explicitamente, valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="6b05a-130">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="6b05a-131">name</span><span class="sxs-lookup"><span data-stu-id="6b05a-131">name</span></span>           |<span data-ttu-id="6b05a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b05a-132">String</span></span>     |<span data-ttu-id="6b05a-133">Nome amigável a humanos do mapeamento de objeto.</span><span class="sxs-lookup"><span data-stu-id="6b05a-133">Human-friendly name of the object mapping.</span></span>|
|<span data-ttu-id="6b05a-134">escopo</span><span class="sxs-lookup"><span data-stu-id="6b05a-134">scope</span></span>          |[<span data-ttu-id="6b05a-135">filter</span><span class="sxs-lookup"><span data-stu-id="6b05a-135">filter</span></span>](synchronization-filter.md)     |<span data-ttu-id="6b05a-136">Define um filtro a ser usado ao decidir se um determinado objeto deve ser provisionado.</span><span class="sxs-lookup"><span data-stu-id="6b05a-136">Defines a filter to be used when deciding whether a given object should be provisioned.</span></span> <span data-ttu-id="6b05a-137">Por exemplo, você talvez queira apenas os usuários de provisão que estão localizados nos EUA.</span><span class="sxs-lookup"><span data-stu-id="6b05a-137">For example, you might want to only provision users that are located in the US.</span></span>|
|<span data-ttu-id="6b05a-138">sourceObjectName</span><span class="sxs-lookup"><span data-stu-id="6b05a-138">sourceObjectName</span></span>           |<span data-ttu-id="6b05a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b05a-139">String</span></span>     |<span data-ttu-id="6b05a-140">Nome do objeto no diretório de origem.</span><span class="sxs-lookup"><span data-stu-id="6b05a-140">Name of the object in the source directory.</span></span> <span data-ttu-id="6b05a-141">Deve corresponder ao nome de objeto a partir da fonte de [definição de diretório](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6b05a-141">Must match the object name from the source [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="6b05a-142">targetObjectName</span><span class="sxs-lookup"><span data-stu-id="6b05a-142">targetObjectName</span></span>           |<span data-ttu-id="6b05a-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b05a-143">String</span></span>     |<span data-ttu-id="6b05a-144">Nome do objeto no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="6b05a-144">Name of the object in target directory.</span></span> <span data-ttu-id="6b05a-145">Deve corresponder ao nome de objeto da [definição do diretório](synchronization-directorydefinition.md)de de destino.</span><span class="sxs-lookup"><span data-stu-id="6b05a-145">Must match the object name from the target [directory definition](synchronization-directorydefinition.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b05a-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b05a-146">JSON representation</span></span>

<span data-ttu-id="6b05a-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b05a-147">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="6b05a-148">Exemplo JSON</span><span class="sxs-lookup"><span data-stu-id="6b05a-148">JSON Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "objectMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
