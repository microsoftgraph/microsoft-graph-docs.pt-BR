---
title: Tipo de recurso privacyProfile
description: Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 52aa1171e8fdc1fb01eae0241306fe197d7b36c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037217"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="e3518-103">Tipo de recurso privacyProfile</span><span class="sxs-lookup"><span data-stu-id="e3518-103">privacyProfile resource type</span></span>

<span data-ttu-id="e3518-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3518-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3518-105">Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e3518-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="e3518-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3518-106">Properties</span></span>
| <span data-ttu-id="e3518-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3518-107">Property</span></span>   | <span data-ttu-id="e3518-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3518-108">Type</span></span>|<span data-ttu-id="e3518-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3518-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3518-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="e3518-110">contactEmail</span></span>|<span data-ttu-id="e3518-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3518-111">String</span></span>| <span data-ttu-id="e3518-112">Um endereço de email smtp válido para o contato da política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e3518-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="e3518-113">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3518-113">Not required.</span></span>|
|<span data-ttu-id="e3518-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="e3518-114">statementUrl</span></span>|<span data-ttu-id="e3518-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3518-115">String</span></span>| <span data-ttu-id="e3518-116">Um formato de URL válido começando por http:// ou https://.</span><span class="sxs-lookup"><span data-stu-id="e3518-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="e3518-117">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="e3518-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="e3518-118">A URL que direciona para a política de privacidade da empresa.</span><span class="sxs-lookup"><span data-stu-id="e3518-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="e3518-119">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3518-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3518-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3518-120">JSON representation</span></span>

<span data-ttu-id="e3518-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e3518-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```

