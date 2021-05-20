---
title: tipo de recurso userFlowLanguageConfiguration
description: Permite que um fluxo de usuário suporte vários idiomas.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 556860eb77c4707f1d180b7924ae3126958a4799
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547201"
---
# <a name="userflowlanguageconfiguration-resource-type"></a><span data-ttu-id="4a49c-103">tipo de recurso userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a49c-103">userFlowLanguageConfiguration resource type</span></span>

<span data-ttu-id="4a49c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a49c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a49c-105">Permite que um fluxo de usuário suporte o uso de vários idiomas.</span><span class="sxs-lookup"><span data-stu-id="4a49c-105">Allows a user flow to support the use of multiple languages.</span></span>

<span data-ttu-id="4a49c-106">Para [Azure Active Directory fluxos de usuários,](/azure/active-directory/external-identities/user-flow-customize-language)você só pode aproveitar os idiomas incorporados fornecidos pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4a49c-106">For [Azure Active Directory user flows](/azure/active-directory/external-identities/user-flow-customize-language), you can only leverage the built-in languages provided by Microsoft.</span></span> <span data-ttu-id="4a49c-107">O usuário flui para Azure Active Directory suporte definindo o idioma e as strings mostradas aos usuários à medida que passam pelas jornadas que você configura com os fluxos do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a49c-107">User flows for Azure Active Directory support defining the language and strings shown to users as they go through the journeys you configure with your user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="4a49c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="4a49c-108">Methods</span></span>

|<span data-ttu-id="4a49c-109">Método</span><span class="sxs-lookup"><span data-stu-id="4a49c-109">Method</span></span>|<span data-ttu-id="4a49c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4a49c-110">Return type</span></span>|<span data-ttu-id="4a49c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a49c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4a49c-112">Obtenha configuração do userFlowLanguage</span><span class="sxs-lookup"><span data-stu-id="4a49c-112">Get userFlowLanguageConfiguration</span></span>](../api/userflowlanguageconfiguration-get.md)|[<span data-ttu-id="4a49c-113">userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a49c-113">userFlowLanguageConfiguration</span></span>](../resources/userflowlanguageconfiguration.md)|<span data-ttu-id="4a49c-114">Leia as propriedades e relacionamentos de um objeto de [Configuração do usuárioFlowLanguage.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a49c-114">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="4a49c-115">Esses objetos representam uma linguagem disponível em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4a49c-115">These objects represent a language available in a user flow.</span></span>|
|[<span data-ttu-id="4a49c-116">Liste páginas padrão</span><span class="sxs-lookup"><span data-stu-id="4a49c-116">List defaultPages</span></span>](../api/userflowlanguageconfiguration-list-defaultpages.md)|<span data-ttu-id="4a49c-117">[coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="4a49c-117">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="4a49c-118">Obtenha os recursos do userFlowLanguagePage da propriedade de navegação padrãoPages.</span><span class="sxs-lookup"><span data-stu-id="4a49c-118">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="4a49c-119">Representa a jornada padrão do usuário em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4a49c-119">Represents the default user journey in a user flow.</span></span>|
|[<span data-ttu-id="4a49c-120">Lista substitui Páginas</span><span class="sxs-lookup"><span data-stu-id="4a49c-120">List overridesPages</span></span>](../api/userflowlanguageconfiguration-list-overridespages.md)|<span data-ttu-id="4a49c-121">[coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="4a49c-121">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="4a49c-122">Obtenha os recursos do userFlowLanguagePage da propriedade de navegação overridesPages.</span><span class="sxs-lookup"><span data-stu-id="4a49c-122">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="4a49c-123">Representa uma experiência personalizada para uma jornada do usuário em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4a49c-123">Represents a custom experience for a user journey in a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="4a49c-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a49c-124">Properties</span></span>

|<span data-ttu-id="4a49c-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a49c-125">Property</span></span>|<span data-ttu-id="4a49c-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a49c-126">Type</span></span>|<span data-ttu-id="4a49c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a49c-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a49c-128">id</span><span class="sxs-lookup"><span data-stu-id="4a49c-128">id</span></span>|<span data-ttu-id="4a49c-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a49c-129">String</span></span>|<span data-ttu-id="4a49c-130">O identificador da linguagem.</span><span class="sxs-lookup"><span data-stu-id="4a49c-130">The identifier of the language.</span></span> <span data-ttu-id="4a49c-131">Este campo é compatível com a tag [RFC 5646](https://tools.ietf.org/html/rfc5646) e deve ser um ID de idioma documentado.</span><span class="sxs-lookup"><span data-stu-id="4a49c-131">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span>|
|<span data-ttu-id="4a49c-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4a49c-132">isEnabled</span></span>|<span data-ttu-id="4a49c-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a49c-133">Boolean</span></span>|<span data-ttu-id="4a49c-134">Indica se o idioma está ativado dentro do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a49c-134">Indicates whether the language is enabled within the user flow.</span></span>|
|<span data-ttu-id="4a49c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4a49c-135">displayName</span></span>|<span data-ttu-id="4a49c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a49c-136">String</span></span>|<span data-ttu-id="4a49c-137">O nome do idioma para exibir.</span><span class="sxs-lookup"><span data-stu-id="4a49c-137">The language name to display.</span></span> <span data-ttu-id="4a49c-138">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a49c-138">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a49c-139">Relações</span><span class="sxs-lookup"><span data-stu-id="4a49c-139">Relationships</span></span>

|<span data-ttu-id="4a49c-140">Relação</span><span class="sxs-lookup"><span data-stu-id="4a49c-140">Relationship</span></span>|<span data-ttu-id="4a49c-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a49c-141">Type</span></span>|<span data-ttu-id="4a49c-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a49c-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a49c-143">páginas padrão</span><span class="sxs-lookup"><span data-stu-id="4a49c-143">defaultPages</span></span>|<span data-ttu-id="4a49c-144">[coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="4a49c-144">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="4a49c-145">Coleção de páginas com o conteúdo padrão para exibir em um fluxo de usuário para um idioma especificado.</span><span class="sxs-lookup"><span data-stu-id="4a49c-145">Collection of pages with the default content to display in a user flow for a specified language.</span></span> <span data-ttu-id="4a49c-146">Esta coleção não permite qualquer tipo de modificação.</span><span class="sxs-lookup"><span data-stu-id="4a49c-146">This collection does not allow any kind of modification.</span></span>|
|<span data-ttu-id="4a49c-147">substitui Páginas</span><span class="sxs-lookup"><span data-stu-id="4a49c-147">overridesPages</span></span>|<span data-ttu-id="4a49c-148">[coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="4a49c-148">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="4a49c-149">A coleção de páginas com as mensagens substituidas para exibir em um fluxo de usuário para um idioma especificado.</span><span class="sxs-lookup"><span data-stu-id="4a49c-149">Collection of pages with the overrides messages to display in a user flow for a specified language.</span></span> <span data-ttu-id="4a49c-150">Esta coleção só permite modificar o conteúdo da página, qualquer outra modificação não é permitida (criação ou exclusão de páginas).</span><span class="sxs-lookup"><span data-stu-id="4a49c-150">This collection only allows to modify the content of the page, any other modification is not allowed (creation or deletion of pages).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a49c-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a49c-151">JSON representation</span></span>

<span data-ttu-id="4a49c-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a49c-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguageConfiguration",
  "id": "String (identifier)",
  "isEnabled": "Boolean",
  "displayName": "String"
}
```
