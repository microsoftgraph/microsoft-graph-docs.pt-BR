---
title: tipo de recurso contratofile
description: Representa um arquivo de contrato de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a6651eafb57d75d6edb6342bd3f382008336332c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974512"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="c88dc-104">tipo de recurso contratofile</span><span class="sxs-lookup"><span data-stu-id="c88dc-104">agreementFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c88dc-105">Representa um arquivo de contrato de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c88dc-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="c88dc-106">Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).</span><span class="sxs-lookup"><span data-stu-id="c88dc-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="c88dc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c88dc-107">Properties</span></span>
| <span data-ttu-id="c88dc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c88dc-108">Property</span></span>     | <span data-ttu-id="c88dc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c88dc-109">Type</span></span>        | <span data-ttu-id="c88dc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c88dc-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c88dc-111">fileData</span><span class="sxs-lookup"><span data-stu-id="c88dc-111">fileData</span></span>|[<span data-ttu-id="c88dc-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="c88dc-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="c88dc-113">Dados que representam o documento PDF termos de uso.</span><span class="sxs-lookup"><span data-stu-id="c88dc-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="c88dc-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c88dc-114">Read-only.</span></span>|
|<span data-ttu-id="c88dc-115">fileName</span><span class="sxs-lookup"><span data-stu-id="c88dc-115">fileName</span></span>|<span data-ttu-id="c88dc-116">String</span><span class="sxs-lookup"><span data-stu-id="c88dc-116">String</span></span>|<span data-ttu-id="c88dc-117">Nome do arquivo de contrato (por exemplo, TOU. pdf).</span><span class="sxs-lookup"><span data-stu-id="c88dc-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="c88dc-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c88dc-118">Read-only.</span></span>|
|<span data-ttu-id="c88dc-119">id</span><span class="sxs-lookup"><span data-stu-id="c88dc-119">id</span></span>|<span data-ttu-id="c88dc-120">String</span><span class="sxs-lookup"><span data-stu-id="c88dc-120">String</span></span>|<span data-ttu-id="c88dc-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c88dc-121">Read-only.</span></span>|
|<span data-ttu-id="c88dc-122">isDefault</span><span class="sxs-lookup"><span data-stu-id="c88dc-122">isDefault</span></span>|<span data-ttu-id="c88dc-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="c88dc-123">Boolean</span></span>|<span data-ttu-id="c88dc-124">Indica se este é o arquivo de contrato padrão se nenhuma das culturas corresponder à preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="c88dc-124">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="c88dc-125">Se nenhum dos arquivos estiver marcado como padrão, o primeiro será tratado como o padrão.</span><span class="sxs-lookup"><span data-stu-id="c88dc-125">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="c88dc-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c88dc-126">Read-only.</span></span>|
|<span data-ttu-id="c88dc-127">idioma</span><span class="sxs-lookup"><span data-stu-id="c88dc-127">language</span></span>|<span data-ttu-id="c88dc-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c88dc-128">String</span></span>|<span data-ttu-id="c88dc-129">Cultura do arquivo de contrato no formato languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="c88dc-129">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="c88dc-130">languagecode2 é um código de duas letras em minúsculas derivado de ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="c88dc-130">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="c88dc-131">Country/regioncode2 é derivado de ISO 3166 e geralmente consiste em duas letras maiúsculas ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="c88dc-131">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="c88dc-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c88dc-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c88dc-133">Relações</span><span class="sxs-lookup"><span data-stu-id="c88dc-133">Relationships</span></span>
<span data-ttu-id="c88dc-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c88dc-134">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c88dc-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c88dc-135">JSON representation</span></span>

<span data-ttu-id="c88dc-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c88dc-136">The following is a JSON representation of the resource.</span></span>

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
