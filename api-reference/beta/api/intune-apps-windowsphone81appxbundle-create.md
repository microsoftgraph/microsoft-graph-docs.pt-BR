---
title: Criar windowsPhone81AppXBundle
description: Crie um novo objeto de windowsPhone81AppXBundle.
author: tfitzmac
ms.openlocfilehash: d1b4c6f92edc6b6b123667ff44f337081550405b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353092"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="1e2b4-103">Criar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="1e2b4-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="1e2b4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e2b4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e2b4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e2b4-107">Crie um novo objeto de [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="1e2b4-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e2b4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e2b4-108">Prerequisites</span></span>
<span data-ttu-id="1e2b4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e2b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e2b4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e2b4-111">Permission type</span></span>|<span data-ttu-id="1e2b4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e2b4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e2b4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e2b4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1e2b4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e2b4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-116">Not supported.</span></span>|
|<span data-ttu-id="1e2b4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e2b4-117">Application</span></span>|<span data-ttu-id="1e2b4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e2b4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e2b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1e2b4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e2b4-120">Request headers</span></span>
|<span data-ttu-id="1e2b4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e2b4-121">Header</span></span>|<span data-ttu-id="1e2b4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1e2b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e2b4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e2b4-123">Authorization</span></span>|<span data-ttu-id="1e2b4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e2b4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e2b4-125">Accept</span></span>|<span data-ttu-id="1e2b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e2b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e2b4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e2b4-127">Request body</span></span>
<span data-ttu-id="1e2b4-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="1e2b4-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="1e2b4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e2b4-130">Property</span></span>|<span data-ttu-id="1e2b4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e2b4-131">Type</span></span>|<span data-ttu-id="1e2b4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e2b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e2b4-133">id</span><span class="sxs-lookup"><span data-stu-id="1e2b4-133">id</span></span>|<span data-ttu-id="1e2b4-134">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-134">String</span></span>|<span data-ttu-id="1e2b4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-135">Key of the entity.</span></span> <span data-ttu-id="1e2b4-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1e2b4-137">displayName</span></span>|<span data-ttu-id="1e2b4-138">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-138">String</span></span>|<span data-ttu-id="1e2b4-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1e2b4-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-141">description</span><span class="sxs-lookup"><span data-stu-id="1e2b4-141">description</span></span>|<span data-ttu-id="1e2b4-142">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-142">String</span></span>|<span data-ttu-id="1e2b4-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-143">The description of the app.</span></span> <span data-ttu-id="1e2b4-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1e2b4-145">publisher</span></span>|<span data-ttu-id="1e2b4-146">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-146">String</span></span>|<span data-ttu-id="1e2b4-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-147">The publisher of the app.</span></span> <span data-ttu-id="1e2b4-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1e2b4-149">largeIcon</span></span>|[<span data-ttu-id="1e2b4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1e2b4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1e2b4-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1e2b4-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e2b4-153">createdDateTime</span></span>|<span data-ttu-id="1e2b4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e2b4-154">DateTimeOffset</span></span>|<span data-ttu-id="1e2b4-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-155">The date and time the app was created.</span></span> <span data-ttu-id="1e2b4-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e2b4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1e2b4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e2b4-158">DateTimeOffset</span></span>|<span data-ttu-id="1e2b4-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1e2b4-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1e2b4-161">isFeatured</span></span>|<span data-ttu-id="1e2b4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e2b4-162">Boolean</span></span>|<span data-ttu-id="1e2b4-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1e2b4-164">privacyInformationUrl</span></span>|<span data-ttu-id="1e2b4-165">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-165">String</span></span>|<span data-ttu-id="1e2b4-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-166">The privacy statement Url.</span></span> <span data-ttu-id="1e2b4-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1e2b4-168">informationUrl</span></span>|<span data-ttu-id="1e2b4-169">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-169">String</span></span>|<span data-ttu-id="1e2b4-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-170">The more information Url.</span></span> <span data-ttu-id="1e2b4-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-172">owner</span><span class="sxs-lookup"><span data-stu-id="1e2b4-172">owner</span></span>|<span data-ttu-id="1e2b4-173">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-173">String</span></span>|<span data-ttu-id="1e2b4-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-174">The owner of the app.</span></span> <span data-ttu-id="1e2b4-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-176">developer</span><span class="sxs-lookup"><span data-stu-id="1e2b4-176">developer</span></span>|<span data-ttu-id="1e2b4-177">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-177">String</span></span>|<span data-ttu-id="1e2b4-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-178">The developer of the app.</span></span> <span data-ttu-id="1e2b4-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-180">Observações</span><span class="sxs-lookup"><span data-stu-id="1e2b4-180">notes</span></span>|<span data-ttu-id="1e2b4-181">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-181">String</span></span>|<span data-ttu-id="1e2b4-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-182">Notes for the app.</span></span> <span data-ttu-id="1e2b4-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1e2b4-184">uploadState</span></span>|<span data-ttu-id="1e2b4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2b4-185">Int32</span></span>|<span data-ttu-id="1e2b4-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-186">The upload state.</span></span> <span data-ttu-id="1e2b4-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e2b4-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1e2b4-188">publishingState</span></span>|[<span data-ttu-id="1e2b4-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1e2b4-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1e2b4-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-190">The publishing state for the app.</span></span> <span data-ttu-id="1e2b4-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1e2b4-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1e2b4-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1e2b4-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1e2b4-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1e2b4-194">committedContentVersion</span></span>|<span data-ttu-id="1e2b4-195">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-195">String</span></span>|<span data-ttu-id="1e2b4-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-196">The internal committed content version.</span></span> <span data-ttu-id="1e2b4-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1e2b4-198">fileName</span><span class="sxs-lookup"><span data-stu-id="1e2b4-198">fileName</span></span>|<span data-ttu-id="1e2b4-199">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-199">String</span></span>|<span data-ttu-id="1e2b4-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-200">The name of the main Lob application file.</span></span> <span data-ttu-id="1e2b4-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1e2b4-202">size</span><span class="sxs-lookup"><span data-stu-id="1e2b4-202">size</span></span>|<span data-ttu-id="1e2b4-203">Int64</span><span class="sxs-lookup"><span data-stu-id="1e2b4-203">Int64</span></span>|<span data-ttu-id="1e2b4-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="1e2b4-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1e2b4-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="1e2b4-206">applicableArchitectures</span></span>|[<span data-ttu-id="1e2b4-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="1e2b4-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="1e2b4-208">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="1e2b4-209">Herdada do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="1e2b4-209">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="1e2b4-210">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="1e2b4-211">identityName</span><span class="sxs-lookup"><span data-stu-id="1e2b4-211">identityName</span></span>|<span data-ttu-id="1e2b4-212">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-212">String</span></span>|<span data-ttu-id="1e2b4-213">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-213">The Identity Name.</span></span> <span data-ttu-id="1e2b4-214">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-214">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1e2b4-215">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="1e2b4-215">identityPublisherHash</span></span>|<span data-ttu-id="1e2b4-216">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-216">String</span></span>|<span data-ttu-id="1e2b4-217">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-217">The Identity Publisher Hash.</span></span> <span data-ttu-id="1e2b4-218">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-218">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1e2b4-219">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1e2b4-219">identityResourceIdentifier</span></span>|<span data-ttu-id="1e2b4-220">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-220">String</span></span>|<span data-ttu-id="1e2b4-221">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-221">The Identity Resource Identifier.</span></span> <span data-ttu-id="1e2b4-222">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1e2b4-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1e2b4-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1e2b4-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1e2b4-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="1e2b4-225">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-225">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="1e2b4-226">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1e2b4-227">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="1e2b4-227">phoneProductIdentifier</span></span>|<span data-ttu-id="1e2b4-228">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-228">String</span></span>|<span data-ttu-id="1e2b4-229">O identificador de produto do telefone.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-229">The Phone Product Identifier.</span></span> <span data-ttu-id="1e2b4-230">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1e2b4-231">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="1e2b4-231">phonePublisherId</span></span>|<span data-ttu-id="1e2b4-232">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-232">String</span></span>|<span data-ttu-id="1e2b4-233">A ID do Publisher. telefone herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-233">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1e2b4-234">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1e2b4-234">identityVersion</span></span>|<span data-ttu-id="1e2b4-235">String</span><span class="sxs-lookup"><span data-stu-id="1e2b4-235">String</span></span>|<span data-ttu-id="1e2b4-236">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-236">The identity version.</span></span> <span data-ttu-id="1e2b4-237">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1e2b4-238">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="1e2b4-238">appXPackageInformationList</span></span>|<span data-ttu-id="1e2b4-239">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-239">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="1e2b4-240">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-240">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="1e2b4-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e2b4-241">Response</span></span>
<span data-ttu-id="1e2b4-242">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-242">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e2b4-243">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e2b4-243">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e2b4-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e2b4-244">Request</span></span>
<span data-ttu-id="1e2b4-245">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-245">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2163

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1e2b4-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e2b4-246">Response</span></span>
<span data-ttu-id="1e2b4-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e2b4-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2271

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```





