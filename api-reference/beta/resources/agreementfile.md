---
title: tipo de recurso contratofile
description: Representa um arquivo de contrato de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 50663ca58323782a14b7e8c5681908aa5a108bdf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067486"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="f8087-104">tipo de recurso contratofile</span><span class="sxs-lookup"><span data-stu-id="f8087-104">agreementFile resource type</span></span>

<span data-ttu-id="f8087-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8087-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8087-106">Representa um arquivo de contrato de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f8087-106">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="f8087-107">Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).</span><span class="sxs-lookup"><span data-stu-id="f8087-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="f8087-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8087-108">Properties</span></span>
| <span data-ttu-id="f8087-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8087-109">Property</span></span>     | <span data-ttu-id="f8087-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8087-110">Type</span></span>        | <span data-ttu-id="f8087-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8087-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f8087-112">fileData</span><span class="sxs-lookup"><span data-stu-id="f8087-112">fileData</span></span>|[<span data-ttu-id="f8087-113">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="f8087-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="f8087-114">Dados que representam o documento PDF termos de uso.</span><span class="sxs-lookup"><span data-stu-id="f8087-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="f8087-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8087-115">Read-only.</span></span>|
|<span data-ttu-id="f8087-116">fileName</span><span class="sxs-lookup"><span data-stu-id="f8087-116">fileName</span></span>|<span data-ttu-id="f8087-117">String</span><span class="sxs-lookup"><span data-stu-id="f8087-117">String</span></span>|<span data-ttu-id="f8087-118">Nome do arquivo de contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="f8087-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="f8087-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8087-119">Read-only.</span></span>|
|<span data-ttu-id="f8087-120">id</span><span class="sxs-lookup"><span data-stu-id="f8087-120">id</span></span>|<span data-ttu-id="f8087-121">String</span><span class="sxs-lookup"><span data-stu-id="f8087-121">String</span></span>|<span data-ttu-id="f8087-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8087-122">Read-only.</span></span>|
|<span data-ttu-id="f8087-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="f8087-123">isDefault</span></span>|<span data-ttu-id="f8087-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="f8087-124">Boolean</span></span>|<span data-ttu-id="f8087-125">Indica se este é o arquivo de contrato padrão se nenhuma das culturas corresponder à preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="f8087-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="f8087-126">Se nenhum dos arquivos estiver marcado como padrão, o primeiro será tratado como o padrão.</span><span class="sxs-lookup"><span data-stu-id="f8087-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="f8087-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8087-127">Read-only.</span></span>|
|<span data-ttu-id="f8087-128">idioma</span><span class="sxs-lookup"><span data-stu-id="f8087-128">language</span></span>|<span data-ttu-id="f8087-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8087-129">String</span></span>|<span data-ttu-id="f8087-130">Cultura do arquivo de contrato no formato languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="f8087-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="f8087-131">languagecode2 é um código de duas letras em minúsculas derivado de ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="f8087-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="f8087-132">Country/regioncode2 é derivado de ISO 3166 e geralmente consiste em duas letras maiúsculas ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="f8087-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="f8087-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8087-133">Read-only.</span></span>|


<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a><span data-ttu-id="f8087-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8087-134">JSON representation</span></span>

<span data-ttu-id="f8087-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8087-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFile"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "language": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


