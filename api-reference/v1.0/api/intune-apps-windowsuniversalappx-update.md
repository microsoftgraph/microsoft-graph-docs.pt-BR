---
title: Atualizar windowsUniversalAppX
description: Atualiza as propriedades de um objeto windowsUniversalAppX.
author: tfitzmac
ms.openlocfilehash: db8badffd6409e920f6783534c741510e755638e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305317"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="54d5a-103">Atualizar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="54d5a-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="54d5a-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="54d5a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54d5a-105">Atualiza as propriedades de um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="54d5a-105">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54d5a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54d5a-106">Prerequisites</span></span>
<span data-ttu-id="54d5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54d5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54d5a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54d5a-109">Permission type</span></span>|<span data-ttu-id="54d5a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54d5a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54d5a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54d5a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="54d5a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d5a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="54d5a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54d5a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54d5a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54d5a-114">Not supported.</span></span>|
|<span data-ttu-id="54d5a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54d5a-115">Application</span></span>|<span data-ttu-id="54d5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54d5a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54d5a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54d5a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="54d5a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54d5a-118">Request headers</span></span>
|<span data-ttu-id="54d5a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54d5a-119">Header</span></span>|<span data-ttu-id="54d5a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="54d5a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54d5a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="54d5a-121">Authorization</span></span>|<span data-ttu-id="54d5a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54d5a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54d5a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="54d5a-123">Accept</span></span>|<span data-ttu-id="54d5a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="54d5a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54d5a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54d5a-125">Request body</span></span>
<span data-ttu-id="54d5a-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="54d5a-126">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="54d5a-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="54d5a-127">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="54d5a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54d5a-128">Property</span></span>|<span data-ttu-id="54d5a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="54d5a-129">Type</span></span>|<span data-ttu-id="54d5a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="54d5a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54d5a-131">id</span><span class="sxs-lookup"><span data-stu-id="54d5a-131">id</span></span>|<span data-ttu-id="54d5a-132">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-132">String</span></span>|<span data-ttu-id="54d5a-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="54d5a-133">Key of the entity.</span></span> <span data-ttu-id="54d5a-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="54d5a-135">displayName</span></span>|<span data-ttu-id="54d5a-136">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-136">String</span></span>|<span data-ttu-id="54d5a-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="54d5a-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="54d5a-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-139">description</span><span class="sxs-lookup"><span data-stu-id="54d5a-139">description</span></span>|<span data-ttu-id="54d5a-140">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-140">String</span></span>|<span data-ttu-id="54d5a-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54d5a-141">The description of the app.</span></span> <span data-ttu-id="54d5a-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-143">publisher</span><span class="sxs-lookup"><span data-stu-id="54d5a-143">publisher</span></span>|<span data-ttu-id="54d5a-144">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-144">String</span></span>|<span data-ttu-id="54d5a-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54d5a-145">The publisher of the app.</span></span> <span data-ttu-id="54d5a-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="54d5a-147">largeIcon</span></span>|[<span data-ttu-id="54d5a-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="54d5a-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="54d5a-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="54d5a-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="54d5a-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54d5a-151">createdDateTime</span></span>|<span data-ttu-id="54d5a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54d5a-152">DateTimeOffset</span></span>|<span data-ttu-id="54d5a-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54d5a-153">The date and time the app was created.</span></span> <span data-ttu-id="54d5a-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54d5a-155">lastModifiedDateTime</span></span>|<span data-ttu-id="54d5a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54d5a-156">DateTimeOffset</span></span>|<span data-ttu-id="54d5a-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="54d5a-157">The date and time the app was last modified.</span></span> <span data-ttu-id="54d5a-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="54d5a-159">isFeatured</span></span>|<span data-ttu-id="54d5a-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="54d5a-160">Boolean</span></span>|<span data-ttu-id="54d5a-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="54d5a-162">privacyInformationUrl</span></span>|<span data-ttu-id="54d5a-163">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-163">String</span></span>|<span data-ttu-id="54d5a-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="54d5a-164">The privacy statement Url.</span></span> <span data-ttu-id="54d5a-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="54d5a-166">informationUrl</span></span>|<span data-ttu-id="54d5a-167">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-167">String</span></span>|<span data-ttu-id="54d5a-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="54d5a-168">The more information Url.</span></span> <span data-ttu-id="54d5a-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-170">owner</span><span class="sxs-lookup"><span data-stu-id="54d5a-170">owner</span></span>|<span data-ttu-id="54d5a-171">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-171">String</span></span>|<span data-ttu-id="54d5a-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="54d5a-172">The owner of the app.</span></span> <span data-ttu-id="54d5a-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-174">developer</span><span class="sxs-lookup"><span data-stu-id="54d5a-174">developer</span></span>|<span data-ttu-id="54d5a-175">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-175">String</span></span>|<span data-ttu-id="54d5a-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54d5a-176">The developer of the app.</span></span> <span data-ttu-id="54d5a-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-178">Observações</span><span class="sxs-lookup"><span data-stu-id="54d5a-178">notes</span></span>|<span data-ttu-id="54d5a-179">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-179">String</span></span>|<span data-ttu-id="54d5a-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54d5a-180">Notes for the app.</span></span> <span data-ttu-id="54d5a-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54d5a-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="54d5a-182">publishingState</span></span>|[<span data-ttu-id="54d5a-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="54d5a-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="54d5a-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54d5a-184">The publishing state for the app.</span></span> <span data-ttu-id="54d5a-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="54d5a-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="54d5a-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54d5a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="54d5a-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="54d5a-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="54d5a-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="54d5a-188">committedContentVersion</span></span>|<span data-ttu-id="54d5a-189">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-189">String</span></span>|<span data-ttu-id="54d5a-190">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="54d5a-190">The internal committed content version.</span></span> <span data-ttu-id="54d5a-191">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="54d5a-192">fileName</span><span class="sxs-lookup"><span data-stu-id="54d5a-192">fileName</span></span>|<span data-ttu-id="54d5a-193">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-193">String</span></span>|<span data-ttu-id="54d5a-194">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="54d5a-194">The name of the main Lob application file.</span></span> <span data-ttu-id="54d5a-195">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="54d5a-196">size</span><span class="sxs-lookup"><span data-stu-id="54d5a-196">size</span></span>|<span data-ttu-id="54d5a-197">Int64</span><span class="sxs-lookup"><span data-stu-id="54d5a-197">Int64</span></span>|<span data-ttu-id="54d5a-198">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="54d5a-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="54d5a-199">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="54d5a-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="54d5a-200">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="54d5a-200">applicableArchitectures</span></span>|[<span data-ttu-id="54d5a-201">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="54d5a-201">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="54d5a-202">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="54d5a-202">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="54d5a-203">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="54d5a-203">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="54d5a-204">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="54d5a-204">applicableDeviceTypes</span></span>|[<span data-ttu-id="54d5a-205">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="54d5a-205">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="54d5a-206">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="54d5a-206">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="54d5a-207">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="54d5a-207">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="54d5a-208">identityName</span><span class="sxs-lookup"><span data-stu-id="54d5a-208">identityName</span></span>|<span data-ttu-id="54d5a-209">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-209">String</span></span>|<span data-ttu-id="54d5a-210">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="54d5a-210">The Identity Name.</span></span>|
|<span data-ttu-id="54d5a-211">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="54d5a-211">identityPublisherHash</span></span>|<span data-ttu-id="54d5a-212">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-212">String</span></span>|<span data-ttu-id="54d5a-213">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="54d5a-213">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="54d5a-214">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="54d5a-214">identityResourceIdentifier</span></span>|<span data-ttu-id="54d5a-215">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-215">String</span></span>|<span data-ttu-id="54d5a-216">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="54d5a-216">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="54d5a-217">isBundle</span><span class="sxs-lookup"><span data-stu-id="54d5a-217">isBundle</span></span>|<span data-ttu-id="54d5a-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="54d5a-218">Boolean</span></span>|<span data-ttu-id="54d5a-219">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="54d5a-219">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="54d5a-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="54d5a-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="54d5a-221">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="54d5a-221">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="54d5a-222">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="54d5a-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="54d5a-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="54d5a-223">identityVersion</span></span>|<span data-ttu-id="54d5a-224">String</span><span class="sxs-lookup"><span data-stu-id="54d5a-224">String</span></span>|<span data-ttu-id="54d5a-225">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="54d5a-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="54d5a-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="54d5a-226">Response</span></span>
<span data-ttu-id="54d5a-227">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54d5a-227">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54d5a-228">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54d5a-228">Example</span></span>
### <a name="request"></a><span data-ttu-id="54d5a-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54d5a-229">Request</span></span>
<span data-ttu-id="54d5a-230">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54d5a-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1189

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
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
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
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="54d5a-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="54d5a-231">Response</span></span>
<span data-ttu-id="54d5a-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54d5a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

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
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```



