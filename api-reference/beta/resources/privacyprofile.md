---
title: Tipo de recurso privacyProfile
description: Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.
localization_priority: Normal
ms.openlocfilehash: adbd2e04e4d3898de559682b0b87158f938e7252
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833044"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="820ab-103">Tipo de recurso privacyProfile</span><span class="sxs-lookup"><span data-stu-id="820ab-103">privacyProfile resource type</span></span>

> <span data-ttu-id="820ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="820ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="820ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="820ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="820ab-106">Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="820ab-106">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="820ab-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="820ab-107">Properties</span></span>
| <span data-ttu-id="820ab-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="820ab-108">Property</span></span>   | <span data-ttu-id="820ab-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="820ab-109">Type</span></span>|<span data-ttu-id="820ab-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="820ab-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="820ab-111">contactEmail</span><span class="sxs-lookup"><span data-stu-id="820ab-111">contactEmail</span></span>|<span data-ttu-id="820ab-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="820ab-112">String</span></span>| <span data-ttu-id="820ab-113">Um endereço de email smtp válido para o contato da política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="820ab-113">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="820ab-114">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="820ab-114">Not required.</span></span>|
|<span data-ttu-id="820ab-115">statementUrl</span><span class="sxs-lookup"><span data-stu-id="820ab-115">statementUrl</span></span>|<span data-ttu-id="820ab-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="820ab-116">String</span></span>| <span data-ttu-id="820ab-117">Um formato de URL válido começando por http:// ou https://.</span><span class="sxs-lookup"><span data-stu-id="820ab-117">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="820ab-118">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="820ab-118">Maximum length is 255 characters.</span></span> <span data-ttu-id="820ab-119">A URL que direciona para a política de privacidade da empresa.</span><span class="sxs-lookup"><span data-stu-id="820ab-119">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="820ab-120">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="820ab-120">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="820ab-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="820ab-121">JSON representation</span></span>

<span data-ttu-id="820ab-122">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="820ab-122">Here is a JSON representation of the resource</span></span>

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
