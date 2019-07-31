---
title: tipo de recurso educationSynchronizationError
description: Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 11e5be9893c6a50615774e0d2a8e4d51c9576da6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972408"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="ab1c3-103">tipo de recurso educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="ab1c3-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab1c3-104">Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ab1c3-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="ab1c3-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ab1c3-105">Methods</span></span>

| <span data-ttu-id="ab1c3-106">Método</span><span class="sxs-lookup"><span data-stu-id="ab1c3-106">Method</span></span> | <span data-ttu-id="ab1c3-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ab1c3-107">Return Type</span></span> | <span data-ttu-id="ab1c3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab1c3-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="ab1c3-109">Obter erros de sincronização</span><span class="sxs-lookup"><span data-stu-id="ab1c3-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="ab1c3-110">coleção **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="ab1c3-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="ab1c3-111">Retorna a lista de erros de sincronização associados a um perfil.</span><span class="sxs-lookup"><span data-stu-id="ab1c3-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="ab1c3-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab1c3-112">Properties</span></span>

| <span data-ttu-id="ab1c3-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab1c3-113">Property</span></span> | <span data-ttu-id="ab1c3-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab1c3-114">Type</span></span> | <span data-ttu-id="ab1c3-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab1c3-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ab1c3-116">**EntryType**</span><span class="sxs-lookup"><span data-stu-id="ab1c3-116">**entryType**</span></span> | <span data-ttu-id="ab1c3-117">string</span><span class="sxs-lookup"><span data-stu-id="ab1c3-117">string</span></span> |  <span data-ttu-id="ab1c3-118">Representa a entidade de sincronização (escola, seção, aluno, professor).</span><span class="sxs-lookup"><span data-stu-id="ab1c3-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="ab1c3-119">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="ab1c3-119">**errorCode**</span></span> | <span data-ttu-id="ab1c3-120">string</span><span class="sxs-lookup"><span data-stu-id="ab1c3-120">string</span></span> |  <span data-ttu-id="ab1c3-121">Representa o código de erro para esse erro.</span><span class="sxs-lookup"><span data-stu-id="ab1c3-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="ab1c3-122">**errorMessage**</span><span class="sxs-lookup"><span data-stu-id="ab1c3-122">**errorMessage**</span></span> | <span data-ttu-id="ab1c3-123">string</span><span class="sxs-lookup"><span data-stu-id="ab1c3-123">string</span></span> |  <span data-ttu-id="ab1c3-124">Contém uma descrição do erro.</span><span class="sxs-lookup"><span data-stu-id="ab1c3-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="ab1c3-125">**unindovalue**</span><span class="sxs-lookup"><span data-stu-id="ab1c3-125">**joiningValue**</span></span> | <span data-ttu-id="ab1c3-126">string</span><span class="sxs-lookup"><span data-stu-id="ab1c3-126">string</span></span> |  <span data-ttu-id="ab1c3-127">O identificador exclusivo da entrada.</span><span class="sxs-lookup"><span data-stu-id="ab1c3-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="ab1c3-128">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ab1c3-128">**recordedDateTime**</span></span> | <span data-ttu-id="ab1c3-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab1c3-129">DateTimeOffset</span></span> | <span data-ttu-id="ab1c3-130">A hora da ocorrência desse erro.</span><span class="sxs-lookup"><span data-stu-id="ab1c3-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="ab1c3-131">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="ab1c3-131">**reportableIdentifier**</span></span> | <span data-ttu-id="ab1c3-132">string</span><span class="sxs-lookup"><span data-stu-id="ab1c3-132">string</span></span> | <span data-ttu-id="ab1c3-133">O identificador desta entrada de erro.</span><span class="sxs-lookup"><span data-stu-id="ab1c3-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="ab1c3-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab1c3-134">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
