---
title: tipo de recurso educationSynchronizationError
description: Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d46d1160ae59174d9fcb4df89559531e3a032e55
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500321"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="a4ef7-103">tipo de recurso educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="a4ef7-103">educationSynchronizationError resource type</span></span>

<span data-ttu-id="a4ef7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a4ef7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4ef7-105">Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a4ef7-105">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="a4ef7-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a4ef7-106">Methods</span></span>

| <span data-ttu-id="a4ef7-107">Método</span><span class="sxs-lookup"><span data-stu-id="a4ef7-107">Method</span></span> | <span data-ttu-id="a4ef7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a4ef7-108">Return Type</span></span> | <span data-ttu-id="a4ef7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4ef7-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="a4ef7-110">Obter erros de sincronização</span><span class="sxs-lookup"><span data-stu-id="a4ef7-110">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="a4ef7-111">coleção **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="a4ef7-111">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="a4ef7-112">Retorna a lista de erros de sincronização associados a um perfil.</span><span class="sxs-lookup"><span data-stu-id="a4ef7-112">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="a4ef7-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4ef7-113">Properties</span></span>

| <span data-ttu-id="a4ef7-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4ef7-114">Property</span></span> | <span data-ttu-id="a4ef7-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4ef7-115">Type</span></span> | <span data-ttu-id="a4ef7-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4ef7-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a4ef7-117">**EntryType**</span><span class="sxs-lookup"><span data-stu-id="a4ef7-117">**entryType**</span></span> | <span data-ttu-id="a4ef7-118">string</span><span class="sxs-lookup"><span data-stu-id="a4ef7-118">string</span></span> |  <span data-ttu-id="a4ef7-119">Representa a entidade de sincronização (escola, seção, aluno, professor).</span><span class="sxs-lookup"><span data-stu-id="a4ef7-119">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="a4ef7-120">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="a4ef7-120">**errorCode**</span></span> | <span data-ttu-id="a4ef7-121">string</span><span class="sxs-lookup"><span data-stu-id="a4ef7-121">string</span></span> |  <span data-ttu-id="a4ef7-122">Representa o código de erro para esse erro.</span><span class="sxs-lookup"><span data-stu-id="a4ef7-122">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="a4ef7-123">**errorMessage**</span><span class="sxs-lookup"><span data-stu-id="a4ef7-123">**errorMessage**</span></span> | <span data-ttu-id="a4ef7-124">string</span><span class="sxs-lookup"><span data-stu-id="a4ef7-124">string</span></span> |  <span data-ttu-id="a4ef7-125">Contém uma descrição do erro.</span><span class="sxs-lookup"><span data-stu-id="a4ef7-125">Contains a description of the error.</span></span>        |
| <span data-ttu-id="a4ef7-126">**unindovalue**</span><span class="sxs-lookup"><span data-stu-id="a4ef7-126">**joiningValue**</span></span> | <span data-ttu-id="a4ef7-127">string</span><span class="sxs-lookup"><span data-stu-id="a4ef7-127">string</span></span> |  <span data-ttu-id="a4ef7-128">O identificador exclusivo da entrada.</span><span class="sxs-lookup"><span data-stu-id="a4ef7-128">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="a4ef7-129">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="a4ef7-129">**recordedDateTime**</span></span> | <span data-ttu-id="a4ef7-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4ef7-130">DateTimeOffset</span></span> | <span data-ttu-id="a4ef7-131">A hora da ocorrência desse erro.</span><span class="sxs-lookup"><span data-stu-id="a4ef7-131">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="a4ef7-132">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="a4ef7-132">**reportableIdentifier**</span></span> | <span data-ttu-id="a4ef7-133">string</span><span class="sxs-lookup"><span data-stu-id="a4ef7-133">string</span></span> | <span data-ttu-id="a4ef7-134">O identificador desta entrada de erro.</span><span class="sxs-lookup"><span data-stu-id="a4ef7-134">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="a4ef7-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4ef7-135">JSON representation</span></span>
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
