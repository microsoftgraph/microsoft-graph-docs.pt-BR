---
title: Tipo de recurso privacyProfile
description: Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: df8fce6758fd7e251dd9358a38a8e602b3b4d1ba
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51467992"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="3544c-103">Tipo de recurso privacyProfile</span><span class="sxs-lookup"><span data-stu-id="3544c-103">privacyProfile resource type</span></span>

<span data-ttu-id="3544c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3544c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3544c-105">Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3544c-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="3544c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3544c-106">Properties</span></span>
| <span data-ttu-id="3544c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3544c-107">Property</span></span>   | <span data-ttu-id="3544c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3544c-108">Type</span></span>|<span data-ttu-id="3544c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3544c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3544c-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="3544c-110">contactEmail</span></span>|<span data-ttu-id="3544c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3544c-111">String</span></span>| <span data-ttu-id="3544c-112">Um endereço de email smtp válido para o contato da política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3544c-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="3544c-113">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3544c-113">Not required.</span></span>|
|<span data-ttu-id="3544c-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="3544c-114">statementUrl</span></span>|<span data-ttu-id="3544c-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3544c-115">String</span></span>| <span data-ttu-id="3544c-116">Um formato de URL válido começando por http:// ou https://.</span><span class="sxs-lookup"><span data-stu-id="3544c-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="3544c-117">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="3544c-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="3544c-118">A URL que direciona para a política de privacidade da empresa.</span><span class="sxs-lookup"><span data-stu-id="3544c-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="3544c-119">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3544c-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3544c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3544c-120">JSON representation</span></span>

<span data-ttu-id="3544c-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3544c-121">Here is a JSON representation of the resource</span></span>

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


