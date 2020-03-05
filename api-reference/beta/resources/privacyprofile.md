---
title: Tipo de recurso privacyProfile
description: Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e43064fe520f100d582e740302a7606c9824b3f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521562"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="7a61c-103">Tipo de recurso privacyProfile</span><span class="sxs-lookup"><span data-stu-id="7a61c-103">privacyProfile resource type</span></span>

<span data-ttu-id="7a61c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7a61c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a61c-105">Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="7a61c-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="7a61c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a61c-106">Properties</span></span>
| <span data-ttu-id="7a61c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a61c-107">Property</span></span>   | <span data-ttu-id="7a61c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a61c-108">Type</span></span>|<span data-ttu-id="7a61c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a61c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a61c-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="7a61c-110">contactEmail</span></span>|<span data-ttu-id="7a61c-111">String</span><span class="sxs-lookup"><span data-stu-id="7a61c-111">String</span></span>| <span data-ttu-id="7a61c-112">Um endereço de email smtp válido para o contato da política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="7a61c-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="7a61c-113">Não necessário.</span><span class="sxs-lookup"><span data-stu-id="7a61c-113">Not required.</span></span>|
|<span data-ttu-id="7a61c-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="7a61c-114">statementUrl</span></span>|<span data-ttu-id="7a61c-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a61c-115">String</span></span>| <span data-ttu-id="7a61c-116">Um formato de URL válido começando por http:// ou https://.</span><span class="sxs-lookup"><span data-stu-id="7a61c-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="7a61c-117">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="7a61c-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="7a61c-118">A URL que direciona para a política de privacidade da empresa.</span><span class="sxs-lookup"><span data-stu-id="7a61c-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="7a61c-119">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a61c-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a61c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a61c-120">JSON representation</span></span>

<span data-ttu-id="7a61c-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7a61c-121">Here is a JSON representation of the resource</span></span>

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
