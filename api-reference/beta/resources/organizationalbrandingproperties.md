---
title: Tipo de recurso organizationalBrandingProperties
description: Contém detalhes da identidade visual da organização.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 719642a606396601c94feaa38ea1cc877c5bd6d6
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547131"
---
# <a name="organizationalbrandingproperties-resource-type"></a><span data-ttu-id="d58af-103">Tipo de recurso organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="d58af-103">organizationalBrandingProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="d58af-104">A adição de identidade visual personalizada exige que você use Azure Active Directory Premium 1, Premium 2 ou edições Básicas ou para ter uma licença Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d58af-104">Adding custom branding requires you to use Azure Active Directory Premium 1, Premium 2, or Basic editions, or to have a Microsoft 365 license.</span></span> <span data-ttu-id="d58af-105">Para obter mais informações sobre licenciamento e edições, consulte [Inscrever-se no Azure AD Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium).</span><span class="sxs-lookup"><span data-stu-id="d58af-105">For more information about licensing and editions, see [Sign up for Azure AD Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium).</span></span><br><br><span data-ttu-id="d58af-106">As edições do Azure AD Premium Basic estão disponíveis para clientes na China usando a instância mundial de Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d58af-106">Azure AD Premium and Basic editions are available for customers in China using the worldwide instance of Azure Active Directory.</span></span> <span data-ttu-id="d58af-107">As edições do Azure AD Premium Basic não têm suporte no serviço do Azure operado pela 21Vianet na China.</span><span class="sxs-lookup"><span data-stu-id="d58af-107">Azure AD Premium and Basic editions aren't currently supported in the Azure service operated by 21Vianet in China.</span></span> <span data-ttu-id="d58af-108">Para obter mais informações, fale conosco usando o [fórum Azure Active Directory fórum](https://feedback.azure.com/forums/169401-azure-active-directory/).</span><span class="sxs-lookup"><span data-stu-id="d58af-108">For more information, talk to us using the [Azure Active Directory Forum](https://feedback.azure.com/forums/169401-azure-active-directory/).</span></span>

<span data-ttu-id="d58af-109">Contém detalhes sobre a identidade visual da organização.</span><span class="sxs-lookup"><span data-stu-id="d58af-109">Contains details about the organization's branding.</span></span>

<span data-ttu-id="d58af-110">As organizações podem personalizar suas páginas de login do Azure AD que aparecem quando os usuários entrar nos aplicativos específicos do locatário da organização ou quando o Azure AD identifica o locatário do usuário do nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="d58af-110">Organizations can customize their Azure AD sign-in pages which appear when users sign in to their organization's tenant-specific apps, or when Azure AD identifies the user's tenant from their username.</span></span> <span data-ttu-id="d58af-111">Um desenvolvedor também pode ler as informações de identidade visual da empresa e personalizar sua experiência de aplicativo para adaptá-la especificamente para o usuário que está assinado usando a identidade visual da empresa.</span><span class="sxs-lookup"><span data-stu-id="d58af-111">A developer can also read the company's branding information and customize their app experience to tailor it specifically for the signed-in user using their company's branding.</span></span>

<span data-ttu-id="d58af-112">As empresas podem adicionar identidade visual diferente com base na localidade.</span><span class="sxs-lookup"><span data-stu-id="d58af-112">Companies can add different branding based on locale.</span></span> <span data-ttu-id="d58af-113">A localidade serve como uma chave em todas as solicitações.</span><span class="sxs-lookup"><span data-stu-id="d58af-113">Locale serves as a key in all requests.</span></span>

><span data-ttu-id="d58af-114">**Observação:** A identidade visual é exposta como uma propriedade sob organização com uma coleção de localizações específicas da localidade.</span><span class="sxs-lookup"><span data-stu-id="d58af-114">**Note:** Branding is exposed as a property under organization with a collection of locale-specific localizations.</span></span> <span data-ttu-id="d58af-115">**organizationalBrandingProperties** é uma classe abstrata que define propriedades para **organizationalBranding**.</span><span class="sxs-lookup"><span data-stu-id="d58af-115">**organizationalBrandingProperties** is an abstract class which defines properties for **organizationalBranding**.</span></span>

## <a name="methods"></a><span data-ttu-id="d58af-116">Métodos</span><span class="sxs-lookup"><span data-stu-id="d58af-116">Methods</span></span>

| <span data-ttu-id="d58af-117">Método</span><span class="sxs-lookup"><span data-stu-id="d58af-117">Method</span></span>       | <span data-ttu-id="d58af-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d58af-118">Return Type</span></span> | <span data-ttu-id="d58af-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d58af-119">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d58af-120">Criar</span><span class="sxs-lookup"><span data-stu-id="d58af-120">Create</span></span>](../api/organizationalbrandingproperties-create.md) | [<span data-ttu-id="d58af-121">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="d58af-121">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="d58af-122">Criar identidade visual organizacional com o objeto organizationalBrandingProperties.</span><span class="sxs-lookup"><span data-stu-id="d58af-122">Create organizational branding with organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="d58af-123">Get</span><span class="sxs-lookup"><span data-stu-id="d58af-123">Get</span></span>](../api/organizationalbrandingproperties-get.md) | [<span data-ttu-id="d58af-124">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="d58af-124">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="d58af-125">Leia propriedades e relações do objeto organizationalBrandingProperties.</span><span class="sxs-lookup"><span data-stu-id="d58af-125">Read properties and relationships of organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="d58af-126">Atualização</span><span class="sxs-lookup"><span data-stu-id="d58af-126">Update</span></span>](../api/organizationalbrandingproperties-update.md) | [<span data-ttu-id="d58af-127">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="d58af-127">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="d58af-128">Atualizar o objeto organizationalBrandingProperties.</span><span class="sxs-lookup"><span data-stu-id="d58af-128">Update organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="d58af-129">Delete</span><span class="sxs-lookup"><span data-stu-id="d58af-129">Delete</span></span>](../api/organizationalbrandingproperties-delete.md) | <span data-ttu-id="d58af-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d58af-130">None</span></span> | <span data-ttu-id="d58af-131">Exclua o objeto organizationalBrandingProperties.</span><span class="sxs-lookup"><span data-stu-id="d58af-131">Delete organizationalBrandingProperties object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d58af-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d58af-132">Properties</span></span>

| <span data-ttu-id="d58af-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d58af-133">Property</span></span>     | <span data-ttu-id="d58af-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="d58af-134">Type</span></span>        | <span data-ttu-id="d58af-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="d58af-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d58af-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="d58af-136">backgroundColor</span></span>|<span data-ttu-id="d58af-137">String</span><span class="sxs-lookup"><span data-stu-id="d58af-137">String</span></span>| <span data-ttu-id="d58af-138">Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="d58af-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="d58af-139">A cor primária do logotipo da faixa ou da cor da sua organização é recomendada para ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="d58af-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="d58af-140">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="d58af-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span> |
|<span data-ttu-id="d58af-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="d58af-141">backgroundImage</span></span>|<span data-ttu-id="d58af-142">Stream</span><span class="sxs-lookup"><span data-stu-id="d58af-142">Stream</span></span>| <span data-ttu-id="d58af-143">Imagem que aparece como o plano de fundo da página de logom.</span><span class="sxs-lookup"><span data-stu-id="d58af-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="d58af-144">.png ou .jpg maior que 1920x1080 e menor que 300kb.</span><span class="sxs-lookup"><span data-stu-id="d58af-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="d58af-145">Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais performant.</span><span class="sxs-lookup"><span data-stu-id="d58af-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span> |
|<span data-ttu-id="d58af-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="d58af-146">bannerLogo</span></span>|<span data-ttu-id="d58af-147">Stream</span><span class="sxs-lookup"><span data-stu-id="d58af-147">Stream</span></span>| <span data-ttu-id="d58af-148">Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="d58af-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="d58af-149">.png ou .jpg maior que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="d58af-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="d58af-150">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="d58af-150">We recommend using a transparent image with no padding around the logo.</span></span> |
|<span data-ttu-id="d58af-151">id</span><span class="sxs-lookup"><span data-stu-id="d58af-151">id</span></span>|<span data-ttu-id="d58af-152">String</span><span class="sxs-lookup"><span data-stu-id="d58af-152">String</span></span>| <span data-ttu-id="d58af-153">Esta é uma id, herdada de microsoft.graph.entity, é a localidade que especifica o padrão ISO 639 para idioma, por exemplo, inglês é "en-us" ou "en".</span><span class="sxs-lookup"><span data-stu-id="d58af-153">This is an id, inherited from microsoft.graph.entity, is the locale specifying the ISO 639 standard for language, for example English is "en-us" or "en".</span></span> <span data-ttu-id="d58af-154">Daqui para frente, se expormos a funcionalidade para ter várias marcas para uma localidade, isso poderá ser alterado.</span><span class="sxs-lookup"><span data-stu-id="d58af-154">Going forward if we expose functionality to have multiple brandings for one locale, this can be changed.</span></span> <span data-ttu-id="d58af-155">Observe que id para Padrão /identidade visual é sempre 'und' até termos singletons sem teclas.</span><span class="sxs-lookup"><span data-stu-id="d58af-155">Note that id for Default /branding is always 'und' until we have keyless singletons.</span></span> <span data-ttu-id="d58af-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d58af-156">Read-only.</span></span> |
|<span data-ttu-id="d58af-157">signInPageText</span><span class="sxs-lookup"><span data-stu-id="d58af-157">signInPageText</span></span>|<span data-ttu-id="d58af-158">String</span><span class="sxs-lookup"><span data-stu-id="d58af-158">String</span></span>| <span data-ttu-id="d58af-159">Texto que aparece na parte inferior da caixa de login.</span><span class="sxs-lookup"><span data-stu-id="d58af-159">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="d58af-160">Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal.</span><span class="sxs-lookup"><span data-stu-id="d58af-160">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="d58af-161">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="d58af-161">This text must be Unicode and not exceed 1024 characters.</span></span> |
|<span data-ttu-id="d58af-162">squareLogo</span><span class="sxs-lookup"><span data-stu-id="d58af-162">squareLogo</span></span>|<span data-ttu-id="d58af-163">Stream</span><span class="sxs-lookup"><span data-stu-id="d58af-163">Stream</span></span>| <span data-ttu-id="d58af-164">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="d58af-164">Square version of your company logo.</span></span> <span data-ttu-id="d58af-165">Isso aparece em Windows 10 experiências OOBE (out-of-box) e quando Windows Autopilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="d58af-165">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="d58af-166">.png ou .jpg maior que 240x240px e não mais de 10kb de tamanho.</span><span class="sxs-lookup"><span data-stu-id="d58af-166">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="d58af-167">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="d58af-167">We recommend using a transparent image with no padding around the logo.</span></span> |
|<span data-ttu-id="d58af-168">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="d58af-168">usernameHintText</span></span>|<span data-ttu-id="d58af-169">String</span><span class="sxs-lookup"><span data-stu-id="d58af-169">String</span></span>| <span data-ttu-id="d58af-170">Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="d58af-170">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="d58af-171">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="d58af-171">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d58af-172">Relações</span><span class="sxs-lookup"><span data-stu-id="d58af-172">Relationships</span></span>

<span data-ttu-id="d58af-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d58af-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d58af-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d58af-174">JSON representation</span></span>

<span data-ttu-id="d58af-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d58af-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationalBrandingProperties",
  "keyProperty": "id"
}-->

```json
{
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "id": "String (identifier)",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationalBrandingProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
