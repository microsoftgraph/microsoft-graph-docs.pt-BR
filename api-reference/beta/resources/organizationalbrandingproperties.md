---
title: tipo de recurso organizationalBrandingProperties
description: Contém detalhes da identidade visual da organização.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b96d4453f07ce317eb41902ed33282d961c74f16
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031889"
---
# <a name="organizationalbrandingproperties-resource-type"></a><span data-ttu-id="94331-103">tipo de recurso organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="94331-103">organizationalBrandingProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="94331-104">A adição de identidade visual personalizada requer que você use as edições 1, Premium 2 ou básica do Azure Active Directory, ou tenha uma licença do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="94331-104">Adding custom branding requires you to use Azure Active Directory Premium 1, Premium 2, or Basic editions, or to have a Microsoft 365 license.</span></span> <span data-ttu-id="94331-105">Para obter mais informações sobre licenciamento e edições, consulte [inscrever-se no Azure ad Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium).</span><span class="sxs-lookup"><span data-stu-id="94331-105">For more information about licensing and editions, see [Sign up for Azure AD Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium).</span></span><br><br><span data-ttu-id="94331-106">O Azure AD Premium e edições básicas estão disponíveis para clientes da China usando a instância Mundial do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="94331-106">Azure AD Premium and Basic editions are available for customers in China using the worldwide instance of Azure Active Directory.</span></span> <span data-ttu-id="94331-107">Atualmente, o Azure AD Premium e o Basic Edition não têm suporte no Azure Service operado pela 21Vianet na China.</span><span class="sxs-lookup"><span data-stu-id="94331-107">Azure AD Premium and Basic editions aren't currently supported in the Azure service operated by 21Vianet in China.</span></span> <span data-ttu-id="94331-108">Para obter mais informações, fale conosco usando o [Fórum do Azure Active Directory](https://feedback.azure.com/forums/169401-azure-active-directory/).</span><span class="sxs-lookup"><span data-stu-id="94331-108">For more information, talk to us using the [Azure Active Directory Forum](https://feedback.azure.com/forums/169401-azure-active-directory/).</span></span>

<span data-ttu-id="94331-109">Contém detalhes sobre a identidade visual da organização.</span><span class="sxs-lookup"><span data-stu-id="94331-109">Contains details about the organization's branding.</span></span>

<span data-ttu-id="94331-110">As organizações podem personalizar suas páginas de entrada do Azure AD que aparecem quando os usuários entram nos aplicativos específicos de locatários da sua organização, ou quando o Azure AD identifica o locatário do usuário de seu nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="94331-110">Organizations can customize their Azure AD sign-in pages which appear when users sign in to their organization's tenant-specific apps, or when Azure AD identifies the user's tenant from their username.</span></span> <span data-ttu-id="94331-111">Um desenvolvedor também pode ler as informações de identidade visual da empresa e personalizar sua experiência de aplicativo para ajustá-la especificamente para o usuário conectado usando a identidade visual da empresa.</span><span class="sxs-lookup"><span data-stu-id="94331-111">A developer can also read the company's branding information and customize their app experience to tailor it specifically for the signed-in user using their company's branding.</span></span>

<span data-ttu-id="94331-112">As empresas podem adicionar diferentes identidade visual com base na localidade.</span><span class="sxs-lookup"><span data-stu-id="94331-112">Companies can add different branding based on locale.</span></span> <span data-ttu-id="94331-113">A localidade serve como uma chave em todas as solicitações.</span><span class="sxs-lookup"><span data-stu-id="94331-113">Locale serves as a key in all requests.</span></span>

><span data-ttu-id="94331-114">**Observação:** A identidade visual é exposta como uma propriedade em organização com uma coleção de localizações específicas de localidade.</span><span class="sxs-lookup"><span data-stu-id="94331-114">**Note:** Branding is exposed as a property under organization with a collection of locale-specific localizations.</span></span> <span data-ttu-id="94331-115">**organizationalBrandingProperties** é uma classe abstrata que define propriedades para **organizationalBranding**.</span><span class="sxs-lookup"><span data-stu-id="94331-115">**organizationalBrandingProperties** is an abstract class which defines properties for **organizationalBranding**.</span></span>

## <a name="methods"></a><span data-ttu-id="94331-116">Métodos</span><span class="sxs-lookup"><span data-stu-id="94331-116">Methods</span></span>

| <span data-ttu-id="94331-117">Método</span><span class="sxs-lookup"><span data-stu-id="94331-117">Method</span></span>       | <span data-ttu-id="94331-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="94331-118">Return Type</span></span> | <span data-ttu-id="94331-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="94331-119">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="94331-120">Create</span><span class="sxs-lookup"><span data-stu-id="94331-120">Create</span></span>](../api/organizationalbrandingproperties-create.md) | [<span data-ttu-id="94331-121">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="94331-121">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="94331-122">Crie uma identidade visual organizacional com o objeto organizationalBrandingProperties.</span><span class="sxs-lookup"><span data-stu-id="94331-122">Create organizational branding with organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="94331-123">Get</span><span class="sxs-lookup"><span data-stu-id="94331-123">Get</span></span>](../api/organizationalbrandingproperties-get.md) | [<span data-ttu-id="94331-124">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="94331-124">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="94331-125">Leia as propriedades e os relacionamentos do objeto organizationalBrandingProperties.</span><span class="sxs-lookup"><span data-stu-id="94331-125">Read properties and relationships of organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="94331-126">Atualização</span><span class="sxs-lookup"><span data-stu-id="94331-126">Update</span></span>](../api/organizationalbrandingproperties-update.md) | [<span data-ttu-id="94331-127">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="94331-127">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="94331-128">Atualize o objeto organizationalBrandingProperties.</span><span class="sxs-lookup"><span data-stu-id="94331-128">Update organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="94331-129">Delete</span><span class="sxs-lookup"><span data-stu-id="94331-129">Delete</span></span>](../api/organizationalbrandingproperties-delete.md) | <span data-ttu-id="94331-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94331-130">None</span></span> | <span data-ttu-id="94331-131">Exclua o objeto organizationalBrandingProperties.</span><span class="sxs-lookup"><span data-stu-id="94331-131">Delete organizationalBrandingProperties object.</span></span> |

## <a name="properties"></a><span data-ttu-id="94331-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94331-132">Properties</span></span>

| <span data-ttu-id="94331-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94331-133">Property</span></span>     | <span data-ttu-id="94331-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="94331-134">Type</span></span>        | <span data-ttu-id="94331-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="94331-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94331-136">CorDoFundo</span><span class="sxs-lookup"><span data-stu-id="94331-136">backgroundColor</span></span>|<span data-ttu-id="94331-137">String</span><span class="sxs-lookup"><span data-stu-id="94331-137">String</span></span>| <span data-ttu-id="94331-138">Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="94331-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="94331-139">É recomendável usar a cor principal do logotipo de faixa ou a cor da sua organização aqui.</span><span class="sxs-lookup"><span data-stu-id="94331-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="94331-140">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="94331-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span> |
|<span data-ttu-id="94331-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="94331-141">backgroundImage</span></span>|<span data-ttu-id="94331-142">Fluxo</span><span class="sxs-lookup"><span data-stu-id="94331-142">Stream</span></span>| <span data-ttu-id="94331-143">Imagem que aparece como plano de fundo da página de entrada.</span><span class="sxs-lookup"><span data-stu-id="94331-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="94331-144">. png ou. jpg não é maior do que 1920 x 1080 e menor do que 300kb.</span><span class="sxs-lookup"><span data-stu-id="94331-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="94331-145">Uma imagem menor reduzirá os requisitos de largura de banda e fará com que as cargas de página mais tenham mais desempenho.</span><span class="sxs-lookup"><span data-stu-id="94331-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span> |
|<span data-ttu-id="94331-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="94331-146">bannerLogo</span></span>|<span data-ttu-id="94331-147">Fluxo</span><span class="sxs-lookup"><span data-stu-id="94331-147">Stream</span></span>| <span data-ttu-id="94331-148">Uma versão de banner do logotipo da empresa que aparece aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="94331-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="94331-149">. png ou. jpg não maior do que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="94331-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="94331-150">Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.</span><span class="sxs-lookup"><span data-stu-id="94331-150">We recommend using a transparent image with no padding around the logo.</span></span> |
|<span data-ttu-id="94331-151">id</span><span class="sxs-lookup"><span data-stu-id="94331-151">id</span></span>|<span data-ttu-id="94331-152">String</span><span class="sxs-lookup"><span data-stu-id="94331-152">String</span></span>| <span data-ttu-id="94331-153">É uma ID, herdada de Microsoft. Graph. Entity, é a localidade que especifica o padrão ISO 639 para o idioma, por exemplo, inglês (en-US) ou "en".</span><span class="sxs-lookup"><span data-stu-id="94331-153">This is an id, inherited from microsoft.graph.entity, is the locale specifying the ISO 639 standard for language, for example English is "en-us" or "en".</span></span> <span data-ttu-id="94331-154">Encaminhar se exportarmos funcionalidade para ter várias marcas para uma localidade, isso pode ser alterado.</span><span class="sxs-lookup"><span data-stu-id="94331-154">Going forward if we expose functionality to have multiple brandings for one locale, this can be changed.</span></span> <span data-ttu-id="94331-155">Observe que a ID do/branding padrão é sempre ' und ' até que haja singleton.</span><span class="sxs-lookup"><span data-stu-id="94331-155">Note that id for Default /branding is always 'und' until we have keyless singletons.</span></span> <span data-ttu-id="94331-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="94331-156">Read-only.</span></span> |
|<span data-ttu-id="94331-157">signInPageText</span><span class="sxs-lookup"><span data-stu-id="94331-157">signInPageText</span></span>|<span data-ttu-id="94331-158">String</span><span class="sxs-lookup"><span data-stu-id="94331-158">String</span></span>| <span data-ttu-id="94331-159">Texto que aparece na parte inferior da caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="94331-159">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="94331-160">Você pode usá-lo para comunicar informações adicionais, como o número de telefone para o suporte técnico ou uma instrução legal.</span><span class="sxs-lookup"><span data-stu-id="94331-160">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="94331-161">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="94331-161">This text must be Unicode and not exceed 1024 characters.</span></span> |
|<span data-ttu-id="94331-162">squareLogo</span><span class="sxs-lookup"><span data-stu-id="94331-162">squareLogo</span></span>|<span data-ttu-id="94331-163">Fluxo</span><span class="sxs-lookup"><span data-stu-id="94331-163">Stream</span></span>| <span data-ttu-id="94331-164">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="94331-164">Square version of your company logo.</span></span> <span data-ttu-id="94331-165">Isso aparece nas experiências de uso (OOBE) do Windows 10 e quando o Windows AutoPilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="94331-165">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="94331-166">. png ou. jpg não maior do que 240x240px e não mais do que 10 KB em tamanho.</span><span class="sxs-lookup"><span data-stu-id="94331-166">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="94331-167">Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.</span><span class="sxs-lookup"><span data-stu-id="94331-167">We recommend using a transparent image with no padding around the logo.</span></span> |
|<span data-ttu-id="94331-168">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="94331-168">usernameHintText</span></span>|<span data-ttu-id="94331-169">String</span><span class="sxs-lookup"><span data-stu-id="94331-169">String</span></span>| <span data-ttu-id="94331-170">Cadeia de caracteres que mostra como a dica na caixa de texto username na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="94331-170">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="94331-171">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="94331-171">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span> |

## <a name="relationships"></a><span data-ttu-id="94331-172">Relações</span><span class="sxs-lookup"><span data-stu-id="94331-172">Relationships</span></span>

<span data-ttu-id="94331-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94331-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94331-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94331-174">JSON representation</span></span>

<span data-ttu-id="94331-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94331-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationalBrandingProperties",
  "baseType": "",
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
