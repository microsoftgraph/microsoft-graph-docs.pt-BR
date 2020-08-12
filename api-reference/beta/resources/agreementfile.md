---
title: tipo de recurso contratofile
description: Representa um arquivo de contrato de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 0f8030680088a99c598d5c3576792583758840d9
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643972"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="c9732-104">tipo de recurso contratofile</span><span class="sxs-lookup"><span data-stu-id="c9732-104">agreementFile resource type</span></span>

<span data-ttu-id="c9732-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9732-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9732-106">Representa um arquivo de contrato de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c9732-106">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="c9732-107">Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).</span><span class="sxs-lookup"><span data-stu-id="c9732-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="c9732-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9732-108">Properties</span></span>
| <span data-ttu-id="c9732-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9732-109">Property</span></span>     | <span data-ttu-id="c9732-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9732-110">Type</span></span>        | <span data-ttu-id="c9732-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9732-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c9732-112">fileData</span><span class="sxs-lookup"><span data-stu-id="c9732-112">fileData</span></span>|[<span data-ttu-id="c9732-113">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="c9732-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="c9732-114">Dados que representam o documento PDF termos de uso.</span><span class="sxs-lookup"><span data-stu-id="c9732-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="c9732-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9732-115">Read-only.</span></span>|
|<span data-ttu-id="c9732-116">fileName</span><span class="sxs-lookup"><span data-stu-id="c9732-116">fileName</span></span>|<span data-ttu-id="c9732-117">String</span><span class="sxs-lookup"><span data-stu-id="c9732-117">String</span></span>|<span data-ttu-id="c9732-118">Nome do arquivo de contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="c9732-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="c9732-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9732-119">Read-only.</span></span>|
|<span data-ttu-id="c9732-120">id</span><span class="sxs-lookup"><span data-stu-id="c9732-120">id</span></span>|<span data-ttu-id="c9732-121">String</span><span class="sxs-lookup"><span data-stu-id="c9732-121">String</span></span>|<span data-ttu-id="c9732-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9732-122">Read-only.</span></span>|
|<span data-ttu-id="c9732-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="c9732-123">isDefault</span></span>|<span data-ttu-id="c9732-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="c9732-124">Boolean</span></span>|<span data-ttu-id="c9732-125">Indica se este é o arquivo de contrato padrão se nenhuma das culturas corresponder à preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="c9732-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="c9732-126">Se nenhum dos arquivos estiver marcado como padrão, o primeiro será tratado como o padrão.</span><span class="sxs-lookup"><span data-stu-id="c9732-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="c9732-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9732-127">Read-only.</span></span>|
|<span data-ttu-id="c9732-128">idioma</span><span class="sxs-lookup"><span data-stu-id="c9732-128">language</span></span>|<span data-ttu-id="c9732-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9732-129">String</span></span>|<span data-ttu-id="c9732-130">Cultura do arquivo de contrato no formato languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="c9732-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="c9732-131">languagecode2 é um código de duas letras em minúsculas derivado de ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="c9732-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="c9732-132">Country/regioncode2 é derivado de ISO 3166 e geralmente consiste em duas letras maiúsculas ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="c9732-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="c9732-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9732-133">Read-only.</span></span>|


<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a><span data-ttu-id="c9732-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9732-134">JSON representation</span></span>

<span data-ttu-id="c9732-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9732-135">The following is a JSON representation of the resource.</span></span>

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
