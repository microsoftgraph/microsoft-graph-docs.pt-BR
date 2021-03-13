---
title: Tipo de recurso passwordSingleSignOnField
description: Campos para capturar as credenciais para SSO de senha
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e0db6198d61715603acee54e7351c9fd5f2fed88
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761546"
---
# <a name="passwordsinglesignonfield-resource-type"></a><span data-ttu-id="a715a-103">Tipo de recurso passwordSingleSignOnField</span><span class="sxs-lookup"><span data-stu-id="a715a-103">passwordSingleSignOnField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a715a-104">Contém os campos a ser capturados para preencher as credenciais de uso para o login único baseado em senha.</span><span class="sxs-lookup"><span data-stu-id="a715a-104">Contains the fields to capture to fill the use credentials for Password-based single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="a715a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a715a-105">Properties</span></span>

| <span data-ttu-id="a715a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a715a-106">Property</span></span>     | <span data-ttu-id="a715a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a715a-107">Type</span></span>        | <span data-ttu-id="a715a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a715a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a715a-109">customizedLabel</span><span class="sxs-lookup"><span data-stu-id="a715a-109">customizedLabel</span></span>|<span data-ttu-id="a715a-110">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a715a-110">String</span></span>|<span data-ttu-id="a715a-111">Substituição de título/rótulo para personalização.</span><span class="sxs-lookup"><span data-stu-id="a715a-111">Title/label override for customization.</span></span>|
|<span data-ttu-id="a715a-112">defaultLabel</span><span class="sxs-lookup"><span data-stu-id="a715a-112">defaultLabel</span></span>|<span data-ttu-id="a715a-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a715a-113">String</span></span>|<span data-ttu-id="a715a-114">Rótulo que seria usado se nenhum rótulo personalizado for fornecido.</span><span class="sxs-lookup"><span data-stu-id="a715a-114">Label that would be used if no customizedLabel is provided.</span></span> <span data-ttu-id="a715a-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a715a-115">Read only.</span></span>|
|<span data-ttu-id="a715a-116">fieldId</span><span class="sxs-lookup"><span data-stu-id="a715a-116">fieldId</span></span>|<span data-ttu-id="a715a-117">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a715a-117">String</span></span>|<span data-ttu-id="a715a-118">ID usada para identificar o tipo de campo.</span><span class="sxs-lookup"><span data-stu-id="a715a-118">Id used to identity the field type.</span></span> <span data-ttu-id="a715a-119">Esta é uma ID interna e os valores possíveis `param_1` são , , , `param_2` `param_userName` `param_password` .</span><span class="sxs-lookup"><span data-stu-id="a715a-119">This is an internal id and possible values are `param_1`, `param_2`, `param_userName`, `param_password`.</span></span>|
|<span data-ttu-id="a715a-120">tipo</span><span class="sxs-lookup"><span data-stu-id="a715a-120">type</span></span>|<span data-ttu-id="a715a-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a715a-121">String</span></span>|   <span data-ttu-id="a715a-122">Tipo da credencial.</span><span class="sxs-lookup"><span data-stu-id="a715a-122">Type of the credential.</span></span> <span data-ttu-id="a715a-123">Os valores podem ser `text` , `password` .</span><span class="sxs-lookup"><span data-stu-id="a715a-123">The values can be `text`, `password`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a715a-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a715a-124">JSON representation</span></span>

<span data-ttu-id="a715a-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a715a-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnField",
  "baseType": null
}-->

```json
{
  "customizedLabel": "String",
  "defaultLabel": "String",
  "fieldId": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

