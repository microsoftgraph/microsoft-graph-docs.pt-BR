---
title: Tipo de recurso agreementFileVersion
description: Representa uma versão personalizada dos arquivos de política localizados de termos de contrato de uso no Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: rajadineshmurugesan-microsoft
ms.openlocfilehash: c590736ea50f589e3f2d87b8d9e0269580f34810
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761734"
---
# <a name="agreementfileversion-resource-type"></a><span data-ttu-id="fbe27-103">Tipo de recurso agreementFileVersion</span><span class="sxs-lookup"><span data-stu-id="fbe27-103">agreementFileVersion resource type</span></span>

<span data-ttu-id="fbe27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbe27-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fbe27-105">Representa uma versão personalizada do arquivo de contrato de termos de uso que um locatário gerencia com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="fbe27-105">Represents a customized version of terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="fbe27-106">Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).</span><span class="sxs-lookup"><span data-stu-id="fbe27-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

## <a name="properties"></a><span data-ttu-id="fbe27-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbe27-107">Properties</span></span>
| <span data-ttu-id="fbe27-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbe27-108">Property</span></span>     | <span data-ttu-id="fbe27-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbe27-109">Type</span></span>        | <span data-ttu-id="fbe27-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbe27-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fbe27-111">fileData</span><span class="sxs-lookup"><span data-stu-id="fbe27-111">fileData</span></span>|[<span data-ttu-id="fbe27-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="fbe27-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="fbe27-113">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="fbe27-113">Data that represents the terms of use PDF document.</span></span> <span data-ttu-id="fbe27-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbe27-114">Read-only.</span></span>|
|<span data-ttu-id="fbe27-115">fileName</span><span class="sxs-lookup"><span data-stu-id="fbe27-115">fileName</span></span>|<span data-ttu-id="fbe27-116">String</span><span class="sxs-lookup"><span data-stu-id="fbe27-116">String</span></span>|<span data-ttu-id="fbe27-117">Nome do arquivo de contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="fbe27-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="fbe27-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbe27-118">Read-only.</span></span>|
|<span data-ttu-id="fbe27-119">id</span><span class="sxs-lookup"><span data-stu-id="fbe27-119">id</span></span>|<span data-ttu-id="fbe27-120">String</span><span class="sxs-lookup"><span data-stu-id="fbe27-120">String</span></span>|<span data-ttu-id="fbe27-121">O identificador do objeto agreementFileVersion.</span><span class="sxs-lookup"><span data-stu-id="fbe27-121">The identifier of the agreementFileVersion object.</span></span> <span data-ttu-id="fbe27-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbe27-122">Read-only.</span></span>|
|<span data-ttu-id="fbe27-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="fbe27-123">isDefault</span></span>|<span data-ttu-id="fbe27-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="fbe27-124">Boolean</span></span>|<span data-ttu-id="fbe27-125">Se nenhum dos idiomas corresponde à preferência do cliente, indica se esse é o arquivo de contrato padrão .</span><span class="sxs-lookup"><span data-stu-id="fbe27-125">If none of the languages matches the client preference, indicates whether this is the default agreement file .</span></span> <span data-ttu-id="fbe27-126">Se nenhum dos arquivos for marcado como padrão, o primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="fbe27-126">If none of the files are marked as default, the first one is treated as the default.</span></span> <span data-ttu-id="fbe27-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbe27-127">Read-only.</span></span>|
|<span data-ttu-id="fbe27-128">idioma</span><span class="sxs-lookup"><span data-stu-id="fbe27-128">language</span></span>|<span data-ttu-id="fbe27-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbe27-129">String</span></span>|<span data-ttu-id="fbe27-130">O idioma do arquivo de contrato no formato languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="fbe27-130">The language of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="fbe27-131">languagecode2 é um código de duas letras minúsculo derivado da ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="fbe27-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="fbe27-132">country/regioncode2 é derivado da ISO 3166 e geralmente consiste em duas letras maiúsculas, ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="fbe27-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="fbe27-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbe27-133">Read-only.</span></span>|
|<span data-ttu-id="fbe27-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="fbe27-134">isMajorVersion</span></span>|<span data-ttu-id="fbe27-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="fbe27-135">Boolean</span></span>|<span data-ttu-id="fbe27-136">Indica se o arquivo de contrato é uma atualização de versão principal.</span><span class="sxs-lookup"><span data-stu-id="fbe27-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="fbe27-137">Atualizações de versão principais invalidam as aceitaçãos do contrato no idioma correspondente.</span><span class="sxs-lookup"><span data-stu-id="fbe27-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="fbe27-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbe27-138">createdDateTime</span></span>|<span data-ttu-id="fbe27-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbe27-139">DateTimeOffset</span></span>|<span data-ttu-id="fbe27-140">A data que representa quando o arquivo foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fbe27-140">The date time representing when the file was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fbe27-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="fbe27-141">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="fbe27-142">displayName</span><span class="sxs-lookup"><span data-stu-id="fbe27-142">displayName</span></span>|<span data-ttu-id="fbe27-143">String</span><span class="sxs-lookup"><span data-stu-id="fbe27-143">String</span></span>|<span data-ttu-id="fbe27-144">Nome de exibição localizado do arquivo de política de um contrato.</span><span class="sxs-lookup"><span data-stu-id="fbe27-144">Localized display name of the policy file of an agreement.</span></span> <span data-ttu-id="fbe27-145">O nome de exibição localizado é mostrado aos usuários finais que visualizam o contrato.</span><span class="sxs-lookup"><span data-stu-id="fbe27-145">The localized display name is shown to end users who view the agreement.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbe27-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbe27-146">JSON representation</span></span>

<span data-ttu-id="fbe27-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbe27-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileVersion"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": "Boolean",
  "language": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
