---
title: tipo de recurso de educationSynchronizationError
description: Representa um erro durante a validação de perfil de dados escola e/ou de sincronização. Será gerado um erro de exclusivo para cada entrada que está falhando para validar e/ou sincronizar com o Azure Active Directory (AD Azure).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 397ac305fcacd789174c05ea36ab026826227475
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425810"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="6edd1-103">tipo de recurso de educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="6edd1-103">educationSynchronizationError resource type</span></span>

> <span data-ttu-id="6edd1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6edd1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6edd1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6edd1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6edd1-106">Representa um erro durante a validação de perfil de dados escola e/ou de sincronização. Será gerado um erro de exclusivo para cada entrada que está falhando para validar e/ou sincronizar com o Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="6edd1-106">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="6edd1-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6edd1-107">Methods</span></span>

| <span data-ttu-id="6edd1-108">Método</span><span class="sxs-lookup"><span data-stu-id="6edd1-108">Method</span></span> | <span data-ttu-id="6edd1-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6edd1-109">Return Type</span></span> | <span data-ttu-id="6edd1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6edd1-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="6edd1-111">Obtenha os erros de sincronização</span><span class="sxs-lookup"><span data-stu-id="6edd1-111">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="6edd1-112">coleção **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="6edd1-112">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="6edd1-113">Retorna a lista de erros de sincronização associado a um perfil.</span><span class="sxs-lookup"><span data-stu-id="6edd1-113">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="6edd1-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6edd1-114">Properties</span></span>

| <span data-ttu-id="6edd1-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6edd1-115">Property</span></span> | <span data-ttu-id="6edd1-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="6edd1-116">Type</span></span> | <span data-ttu-id="6edd1-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="6edd1-117">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6edd1-118">**entryType**</span><span class="sxs-lookup"><span data-stu-id="6edd1-118">**entryType**</span></span> | <span data-ttu-id="6edd1-119">string</span><span class="sxs-lookup"><span data-stu-id="6edd1-119">string</span></span> |  <span data-ttu-id="6edd1-120">Representa a entidade de sincronização (escola, seção, estudante, professor).</span><span class="sxs-lookup"><span data-stu-id="6edd1-120">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="6edd1-121">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="6edd1-121">**errorCode**</span></span> | <span data-ttu-id="6edd1-122">string</span><span class="sxs-lookup"><span data-stu-id="6edd1-122">string</span></span> |  <span data-ttu-id="6edd1-123">Representa o código de erro para esse erro.</span><span class="sxs-lookup"><span data-stu-id="6edd1-123">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="6edd1-124">**errorMessage**</span><span class="sxs-lookup"><span data-stu-id="6edd1-124">**errorMessage**</span></span> | <span data-ttu-id="6edd1-125">string</span><span class="sxs-lookup"><span data-stu-id="6edd1-125">string</span></span> |  <span data-ttu-id="6edd1-126">Contém uma descrição do erro.</span><span class="sxs-lookup"><span data-stu-id="6edd1-126">Contains a description of the error.</span></span>        |
| <span data-ttu-id="6edd1-127">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="6edd1-127">**joiningValue**</span></span> | <span data-ttu-id="6edd1-128">string</span><span class="sxs-lookup"><span data-stu-id="6edd1-128">string</span></span> |  <span data-ttu-id="6edd1-129">O identificador exclusivo para a entrada.</span><span class="sxs-lookup"><span data-stu-id="6edd1-129">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="6edd1-130">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="6edd1-130">**recordedDateTime**</span></span> | <span data-ttu-id="6edd1-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6edd1-131">DateTimeOffset</span></span> | <span data-ttu-id="6edd1-132">A hora da ocorrência desse erro.</span><span class="sxs-lookup"><span data-stu-id="6edd1-132">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="6edd1-133">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="6edd1-133">**reportableIdentifier**</span></span> | <span data-ttu-id="6edd1-134">string</span><span class="sxs-lookup"><span data-stu-id="6edd1-134">string</span></span> | <span data-ttu-id="6edd1-135">O identificador dessa entrada de erro.</span><span class="sxs-lookup"><span data-stu-id="6edd1-135">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="6edd1-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6edd1-136">JSON representation</span></span>
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
