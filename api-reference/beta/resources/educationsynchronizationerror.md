---
title: tipo de recurso de educationSynchronizationError
description: Representa um erro durante a validação de perfil de dados escola e/ou de sincronização. Será gerado um erro de exclusivo para cada entrada que está falhando para validar e/ou sincronizar com o Azure Active Directory (AD Azure).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525140"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="8fa06-103">tipo de recurso de educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="8fa06-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fa06-104">Representa um erro durante a validação de perfil de dados escola e/ou de sincronização. Será gerado um erro de exclusivo para cada entrada que está falhando para validar e/ou sincronizar com o Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="8fa06-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="8fa06-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="8fa06-105">Methods</span></span>

| <span data-ttu-id="8fa06-106">Método</span><span class="sxs-lookup"><span data-stu-id="8fa06-106">Method</span></span> | <span data-ttu-id="8fa06-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8fa06-107">Return Type</span></span> | <span data-ttu-id="8fa06-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fa06-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="8fa06-109">Obtenha os erros de sincronização</span><span class="sxs-lookup"><span data-stu-id="8fa06-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="8fa06-110">coleção **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="8fa06-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="8fa06-111">Retorna a lista de erros de sincronização associado a um perfil.</span><span class="sxs-lookup"><span data-stu-id="8fa06-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="8fa06-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8fa06-112">Properties</span></span>

| <span data-ttu-id="8fa06-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fa06-113">Property</span></span> | <span data-ttu-id="8fa06-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fa06-114">Type</span></span> | <span data-ttu-id="8fa06-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fa06-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8fa06-116">**entryType**</span><span class="sxs-lookup"><span data-stu-id="8fa06-116">**entryType**</span></span> | <span data-ttu-id="8fa06-117">string</span><span class="sxs-lookup"><span data-stu-id="8fa06-117">string</span></span> |  <span data-ttu-id="8fa06-118">Representa a entidade de sincronização (escola, seção, estudante, professor).</span><span class="sxs-lookup"><span data-stu-id="8fa06-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="8fa06-119">**ErrorCode**</span><span class="sxs-lookup"><span data-stu-id="8fa06-119">**errorCode**</span></span> | <span data-ttu-id="8fa06-120">string</span><span class="sxs-lookup"><span data-stu-id="8fa06-120">string</span></span> |  <span data-ttu-id="8fa06-121">Representa o código de erro para esse erro.</span><span class="sxs-lookup"><span data-stu-id="8fa06-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="8fa06-122">**ErrorMessage**</span><span class="sxs-lookup"><span data-stu-id="8fa06-122">**errorMessage**</span></span> | <span data-ttu-id="8fa06-123">string</span><span class="sxs-lookup"><span data-stu-id="8fa06-123">string</span></span> |  <span data-ttu-id="8fa06-124">Contém uma descrição do erro.</span><span class="sxs-lookup"><span data-stu-id="8fa06-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="8fa06-125">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="8fa06-125">**joiningValue**</span></span> | <span data-ttu-id="8fa06-126">string</span><span class="sxs-lookup"><span data-stu-id="8fa06-126">string</span></span> |  <span data-ttu-id="8fa06-127">O identificador exclusivo para a entrada.</span><span class="sxs-lookup"><span data-stu-id="8fa06-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="8fa06-128">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fa06-128">**recordedDateTime**</span></span> | <span data-ttu-id="8fa06-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fa06-129">DateTimeOffset</span></span> | <span data-ttu-id="8fa06-130">A hora da ocorrência desse erro.</span><span class="sxs-lookup"><span data-stu-id="8fa06-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="8fa06-131">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="8fa06-131">**reportableIdentifier**</span></span> | <span data-ttu-id="8fa06-132">string</span><span class="sxs-lookup"><span data-stu-id="8fa06-132">string</span></span> | <span data-ttu-id="8fa06-133">O identificador dessa entrada de erro.</span><span class="sxs-lookup"><span data-stu-id="8fa06-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="8fa06-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8fa06-134">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
