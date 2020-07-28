---
title: tipo de recurso educationFileSynchronizationVerificationMessage
description: Representa um erro retornado ao cliente em resposta a uma solicitação para iniciar a sincronização de perfis de dados escolares baseados em CSV. O recurso conterá erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8e82ede1df5c17b99fdc40857fd97f1f90012711
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434974"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="f78b5-105">tipo de recurso educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="f78b5-105">educationFileSynchronizationVerificationMessage resource type</span></span>

<span data-ttu-id="f78b5-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f78b5-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f78b5-107">Representa um erro retornado ao cliente em resposta a uma solicitação para [iniciar a sincronização](../api/educationsynchronizationprofile-start.md) de perfis de dados escolares baseados em CSV.</span><span class="sxs-lookup"><span data-stu-id="f78b5-107">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="f78b5-108">O recurso conterá erros resultantes da verificação.</span><span class="sxs-lookup"><span data-stu-id="f78b5-108">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="f78b5-109">Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f78b5-109">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="f78b5-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f78b5-110">Properties</span></span>

| <span data-ttu-id="f78b5-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f78b5-111">Property</span></span>    | <span data-ttu-id="f78b5-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="f78b5-112">Type</span></span>   | <span data-ttu-id="f78b5-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f78b5-113">Description</span></span>                                                                  |
| :---------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="f78b5-114">type</span><span class="sxs-lookup"><span data-stu-id="f78b5-114">type</span></span>        | <span data-ttu-id="f78b5-115">string</span><span class="sxs-lookup"><span data-stu-id="f78b5-115">string</span></span> | <span data-ttu-id="f78b5-116">Tipo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="f78b5-116">Type of the message.</span></span> <span data-ttu-id="f78b5-117">Os valores possíveis são: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="f78b5-117">Possible values are: `error`, `warning`, `information`.</span></span> |
| <span data-ttu-id="f78b5-118">nomes</span><span class="sxs-lookup"><span data-stu-id="f78b5-118">filename</span></span>    | <span data-ttu-id="f78b5-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f78b5-119">string</span></span> | <span data-ttu-id="f78b5-120">Arquivo de origem que contém o erro.</span><span class="sxs-lookup"><span data-stu-id="f78b5-120">Source file that contains the error.</span></span>                                         |
| <span data-ttu-id="f78b5-121">description</span><span class="sxs-lookup"><span data-stu-id="f78b5-121">description</span></span> | <span data-ttu-id="f78b5-122">string</span><span class="sxs-lookup"><span data-stu-id="f78b5-122">string</span></span> | <span data-ttu-id="f78b5-123">Informações detalhadas sobre o tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="f78b5-123">Detailed information about the message type.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="f78b5-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f78b5-124">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
  "type": "String",
  "fileName": "String",
  "description": "String"
}
```
