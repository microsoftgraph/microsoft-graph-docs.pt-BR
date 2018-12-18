---
title: Criar windowsUniversalAppX
description: Cria um novo objeto windowsUniversalAppX.
author: tfitzmac
ms.openlocfilehash: 27fc37804da09f2740f0cfcf6548de529d82fbd9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360211"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="0d078-103">Criar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="0d078-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="0d078-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0d078-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d078-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0d078-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d078-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0d078-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d078-107">Cria um novo objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="0d078-107">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d078-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d078-108">Prerequisites</span></span>
<span data-ttu-id="0d078-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d078-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d078-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d078-111">Permission type</span></span>|<span data-ttu-id="0d078-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d078-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d078-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d078-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d078-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d078-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d078-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d078-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d078-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d078-116">Not supported.</span></span>|
|<span data-ttu-id="0d078-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d078-117">Application</span></span>|<span data-ttu-id="0d078-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d078-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d078-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d078-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0d078-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d078-120">Request headers</span></span>
|<span data-ttu-id="0d078-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d078-121">Header</span></span>|<span data-ttu-id="0d078-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0d078-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d078-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d078-123">Authorization</span></span>|<span data-ttu-id="0d078-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d078-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d078-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0d078-125">Accept</span></span>|<span data-ttu-id="0d078-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d078-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d078-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d078-127">Request body</span></span>
<span data-ttu-id="0d078-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="0d078-128">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="0d078-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="0d078-129">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="0d078-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d078-130">Property</span></span>|<span data-ttu-id="0d078-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d078-131">Type</span></span>|<span data-ttu-id="0d078-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d078-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d078-133">id</span><span class="sxs-lookup"><span data-stu-id="0d078-133">id</span></span>|<span data-ttu-id="0d078-134">String</span><span class="sxs-lookup"><span data-stu-id="0d078-134">String</span></span>|<span data-ttu-id="0d078-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0d078-135">Key of the entity.</span></span> <span data-ttu-id="0d078-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0d078-137">displayName</span></span>|<span data-ttu-id="0d078-138">String</span><span class="sxs-lookup"><span data-stu-id="0d078-138">String</span></span>|<span data-ttu-id="0d078-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0d078-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0d078-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-141">description</span><span class="sxs-lookup"><span data-stu-id="0d078-141">description</span></span>|<span data-ttu-id="0d078-142">String</span><span class="sxs-lookup"><span data-stu-id="0d078-142">String</span></span>|<span data-ttu-id="0d078-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0d078-143">The description of the app.</span></span> <span data-ttu-id="0d078-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-145">publisher</span><span class="sxs-lookup"><span data-stu-id="0d078-145">publisher</span></span>|<span data-ttu-id="0d078-146">String</span><span class="sxs-lookup"><span data-stu-id="0d078-146">String</span></span>|<span data-ttu-id="0d078-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0d078-147">The publisher of the app.</span></span> <span data-ttu-id="0d078-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0d078-149">largeIcon</span></span>|[<span data-ttu-id="0d078-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0d078-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0d078-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0d078-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0d078-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d078-153">createdDateTime</span></span>|<span data-ttu-id="0d078-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d078-154">DateTimeOffset</span></span>|<span data-ttu-id="0d078-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0d078-155">The date and time the app was created.</span></span> <span data-ttu-id="0d078-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d078-157">lastModifiedDateTime</span></span>|<span data-ttu-id="0d078-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d078-158">DateTimeOffset</span></span>|<span data-ttu-id="0d078-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0d078-159">The date and time the app was last modified.</span></span> <span data-ttu-id="0d078-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0d078-161">isFeatured</span></span>|<span data-ttu-id="0d078-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d078-162">Boolean</span></span>|<span data-ttu-id="0d078-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0d078-164">privacyInformationUrl</span></span>|<span data-ttu-id="0d078-165">String</span><span class="sxs-lookup"><span data-stu-id="0d078-165">String</span></span>|<span data-ttu-id="0d078-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0d078-166">The privacy statement Url.</span></span> <span data-ttu-id="0d078-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0d078-168">informationUrl</span></span>|<span data-ttu-id="0d078-169">String</span><span class="sxs-lookup"><span data-stu-id="0d078-169">String</span></span>|<span data-ttu-id="0d078-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0d078-170">The more information Url.</span></span> <span data-ttu-id="0d078-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-172">owner</span><span class="sxs-lookup"><span data-stu-id="0d078-172">owner</span></span>|<span data-ttu-id="0d078-173">String</span><span class="sxs-lookup"><span data-stu-id="0d078-173">String</span></span>|<span data-ttu-id="0d078-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0d078-174">The owner of the app.</span></span> <span data-ttu-id="0d078-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-176">developer</span><span class="sxs-lookup"><span data-stu-id="0d078-176">developer</span></span>|<span data-ttu-id="0d078-177">String</span><span class="sxs-lookup"><span data-stu-id="0d078-177">String</span></span>|<span data-ttu-id="0d078-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0d078-178">The developer of the app.</span></span> <span data-ttu-id="0d078-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-180">Observações</span><span class="sxs-lookup"><span data-stu-id="0d078-180">notes</span></span>|<span data-ttu-id="0d078-181">String</span><span class="sxs-lookup"><span data-stu-id="0d078-181">String</span></span>|<span data-ttu-id="0d078-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0d078-182">Notes for the app.</span></span> <span data-ttu-id="0d078-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="0d078-184">uploadState</span></span>|<span data-ttu-id="0d078-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0d078-185">Int32</span></span>|<span data-ttu-id="0d078-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="0d078-186">The upload state.</span></span> <span data-ttu-id="0d078-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0d078-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="0d078-188">publishingState</span></span>|[<span data-ttu-id="0d078-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0d078-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0d078-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0d078-190">The publishing state for the app.</span></span> <span data-ttu-id="0d078-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="0d078-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0d078-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d078-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0d078-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0d078-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0d078-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0d078-194">committedContentVersion</span></span>|<span data-ttu-id="0d078-195">String</span><span class="sxs-lookup"><span data-stu-id="0d078-195">String</span></span>|<span data-ttu-id="0d078-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="0d078-196">The internal committed content version.</span></span> <span data-ttu-id="0d078-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0d078-198">fileName</span><span class="sxs-lookup"><span data-stu-id="0d078-198">fileName</span></span>|<span data-ttu-id="0d078-199">String</span><span class="sxs-lookup"><span data-stu-id="0d078-199">String</span></span>|<span data-ttu-id="0d078-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="0d078-200">The name of the main Lob application file.</span></span> <span data-ttu-id="0d078-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0d078-202">size</span><span class="sxs-lookup"><span data-stu-id="0d078-202">size</span></span>|<span data-ttu-id="0d078-203">Int64</span><span class="sxs-lookup"><span data-stu-id="0d078-203">Int64</span></span>|<span data-ttu-id="0d078-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="0d078-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="0d078-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0d078-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0d078-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="0d078-206">applicableArchitectures</span></span>|[<span data-ttu-id="0d078-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="0d078-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="0d078-208">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="0d078-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="0d078-209">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="0d078-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="0d078-210">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="0d078-210">applicableDeviceTypes</span></span>|[<span data-ttu-id="0d078-211">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="0d078-211">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="0d078-212">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="0d078-212">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="0d078-213">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="0d078-213">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="0d078-214">identityName</span><span class="sxs-lookup"><span data-stu-id="0d078-214">identityName</span></span>|<span data-ttu-id="0d078-215">String</span><span class="sxs-lookup"><span data-stu-id="0d078-215">String</span></span>|<span data-ttu-id="0d078-216">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="0d078-216">The Identity Name.</span></span>|
|<span data-ttu-id="0d078-217">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="0d078-217">identityPublisherHash</span></span>|<span data-ttu-id="0d078-218">String</span><span class="sxs-lookup"><span data-stu-id="0d078-218">String</span></span>|<span data-ttu-id="0d078-219">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="0d078-219">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="0d078-220">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0d078-220">identityResourceIdentifier</span></span>|<span data-ttu-id="0d078-221">String</span><span class="sxs-lookup"><span data-stu-id="0d078-221">String</span></span>|<span data-ttu-id="0d078-222">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="0d078-222">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="0d078-223">isBundle</span><span class="sxs-lookup"><span data-stu-id="0d078-223">isBundle</span></span>|<span data-ttu-id="0d078-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d078-224">Boolean</span></span>|<span data-ttu-id="0d078-225">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="0d078-225">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="0d078-226">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0d078-226">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0d078-227">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0d078-227">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="0d078-228">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="0d078-228">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="0d078-229">identityVersion</span><span class="sxs-lookup"><span data-stu-id="0d078-229">identityVersion</span></span>|<span data-ttu-id="0d078-230">String</span><span class="sxs-lookup"><span data-stu-id="0d078-230">String</span></span>|<span data-ttu-id="0d078-231">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="0d078-231">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="0d078-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d078-232">Response</span></span>
<span data-ttu-id="0d078-233">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d078-233">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d078-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d078-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d078-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d078-235">Request</span></span>
<span data-ttu-id="0d078-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d078-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1367

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="0d078-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d078-237">Response</span></span>
<span data-ttu-id="0d078-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d078-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1475

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```





