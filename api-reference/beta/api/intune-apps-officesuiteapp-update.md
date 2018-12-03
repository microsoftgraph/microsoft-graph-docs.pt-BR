---
title: Atualizar officeSuiteApp
description: Atualize as propriedades de um objeto officeSuiteApp.
ms.openlocfilehash: b98a7da8d268894adce8c9f5bb9790c924e8b64c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034404"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="e49f4-103">Atualizar officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="e49f4-103">Update officeSuiteApp</span></span>

> <span data-ttu-id="e49f4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e49f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e49f4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e49f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e49f4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e49f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e49f4-107">Atualize as propriedades de um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e49f4-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e49f4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e49f4-108">Prerequisites</span></span>
<span data-ttu-id="e49f4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e49f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e49f4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e49f4-111">Permission type</span></span>|<span data-ttu-id="e49f4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e49f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e49f4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e49f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e49f4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e49f4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e49f4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e49f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e49f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e49f4-116">Not supported.</span></span>|
|<span data-ttu-id="e49f4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e49f4-117">Application</span></span>|<span data-ttu-id="e49f4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e49f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e49f4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e49f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e49f4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e49f4-120">Request headers</span></span>
|<span data-ttu-id="e49f4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e49f4-121">Header</span></span>|<span data-ttu-id="e49f4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e49f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e49f4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e49f4-123">Authorization</span></span>|<span data-ttu-id="e49f4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e49f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e49f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e49f4-125">Accept</span></span>|<span data-ttu-id="e49f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e49f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e49f4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e49f4-127">Request body</span></span>
<span data-ttu-id="e49f4-128">No corpo da solicitação, fornece uma representação JSON para o objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e49f4-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="e49f4-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="e49f4-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="e49f4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e49f4-130">Property</span></span>|<span data-ttu-id="e49f4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e49f4-131">Type</span></span>|<span data-ttu-id="e49f4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e49f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e49f4-133">id</span><span class="sxs-lookup"><span data-stu-id="e49f4-133">id</span></span>|<span data-ttu-id="e49f4-134">String</span><span class="sxs-lookup"><span data-stu-id="e49f4-134">String</span></span>|<span data-ttu-id="e49f4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e49f4-135">Key of the entity.</span></span> <span data-ttu-id="e49f4-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e49f4-137">displayName</span></span>|<span data-ttu-id="e49f4-138">String</span><span class="sxs-lookup"><span data-stu-id="e49f4-138">String</span></span>|<span data-ttu-id="e49f4-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e49f4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e49f4-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-141">description</span><span class="sxs-lookup"><span data-stu-id="e49f4-141">description</span></span>|<span data-ttu-id="e49f4-142">String</span><span class="sxs-lookup"><span data-stu-id="e49f4-142">String</span></span>|<span data-ttu-id="e49f4-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e49f4-143">The description of the app.</span></span> <span data-ttu-id="e49f4-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e49f4-145">publisher</span></span>|<span data-ttu-id="e49f4-146">String</span><span class="sxs-lookup"><span data-stu-id="e49f4-146">String</span></span>|<span data-ttu-id="e49f4-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e49f4-147">The publisher of the app.</span></span> <span data-ttu-id="e49f4-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e49f4-149">largeIcon</span></span>|[<span data-ttu-id="e49f4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e49f4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e49f4-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e49f4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e49f4-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e49f4-153">createdDateTime</span></span>|<span data-ttu-id="e49f4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e49f4-154">DateTimeOffset</span></span>|<span data-ttu-id="e49f4-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e49f4-155">The date and time the app was created.</span></span> <span data-ttu-id="e49f4-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e49f4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e49f4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e49f4-158">DateTimeOffset</span></span>|<span data-ttu-id="e49f4-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e49f4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e49f4-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e49f4-161">isFeatured</span></span>|<span data-ttu-id="e49f4-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="e49f4-162">Boolean</span></span>|<span data-ttu-id="e49f4-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e49f4-164">privacyInformationUrl</span></span>|<span data-ttu-id="e49f4-165">String</span><span class="sxs-lookup"><span data-stu-id="e49f4-165">String</span></span>|<span data-ttu-id="e49f4-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e49f4-166">The privacy statement Url.</span></span> <span data-ttu-id="e49f4-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e49f4-168">informationUrl</span></span>|<span data-ttu-id="e49f4-169">String</span><span class="sxs-lookup"><span data-stu-id="e49f4-169">String</span></span>|<span data-ttu-id="e49f4-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e49f4-170">The more information Url.</span></span> <span data-ttu-id="e49f4-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-172">owner</span><span class="sxs-lookup"><span data-stu-id="e49f4-172">owner</span></span>|<span data-ttu-id="e49f4-173">String</span><span class="sxs-lookup"><span data-stu-id="e49f4-173">String</span></span>|<span data-ttu-id="e49f4-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e49f4-174">The owner of the app.</span></span> <span data-ttu-id="e49f4-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-176">developer</span><span class="sxs-lookup"><span data-stu-id="e49f4-176">developer</span></span>|<span data-ttu-id="e49f4-177">String</span><span class="sxs-lookup"><span data-stu-id="e49f4-177">String</span></span>|<span data-ttu-id="e49f4-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e49f4-178">The developer of the app.</span></span> <span data-ttu-id="e49f4-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-180">Observações</span><span class="sxs-lookup"><span data-stu-id="e49f4-180">notes</span></span>|<span data-ttu-id="e49f4-181">String</span><span class="sxs-lookup"><span data-stu-id="e49f4-181">String</span></span>|<span data-ttu-id="e49f4-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e49f4-182">Notes for the app.</span></span> <span data-ttu-id="e49f4-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e49f4-184">uploadState</span></span>|<span data-ttu-id="e49f4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e49f4-185">Int32</span></span>|<span data-ttu-id="e49f4-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="e49f4-186">The upload state.</span></span> <span data-ttu-id="e49f4-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e49f4-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="e49f4-188">publishingState</span></span>|[<span data-ttu-id="e49f4-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e49f4-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e49f4-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e49f4-190">The publishing state for the app.</span></span> <span data-ttu-id="e49f4-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e49f4-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e49f4-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e49f4-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e49f4-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e49f4-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e49f4-194">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="e49f4-194">autoAcceptEula</span></span>|<span data-ttu-id="e49f4-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="e49f4-195">Boolean</span></span>|<span data-ttu-id="e49f4-196">O valor para aceitar o EULA automaticamente no dispositivo do usuário final.</span><span class="sxs-lookup"><span data-stu-id="e49f4-196">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="e49f4-197">productIds</span><span class="sxs-lookup"><span data-stu-id="e49f4-197">productIds</span></span>|<span data-ttu-id="e49f4-198">coleção [officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="e49f4-198">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="e49f4-199">As Ids de produto que representam a SKU do pacote Office365.</span><span class="sxs-lookup"><span data-stu-id="e49f4-199">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="e49f4-200">Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="e49f4-200">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="e49f4-201">excludedApps</span><span class="sxs-lookup"><span data-stu-id="e49f4-201">excludedApps</span></span>|[<span data-ttu-id="e49f4-202">excludedApps</span><span class="sxs-lookup"><span data-stu-id="e49f4-202">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="e49f4-203">A propriedade para representar os aplicativos que são excluídos do produto selecionado Office365 ID.</span><span class="sxs-lookup"><span data-stu-id="e49f4-203">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="e49f4-204">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="e49f4-204">useSharedComputerActivation</span></span>|<span data-ttu-id="e49f4-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="e49f4-205">Boolean</span></span>|<span data-ttu-id="e49f4-206">A propriedade para representar que se a ativação do computador compartilhado é usada não para o pacote do app Office365.</span><span class="sxs-lookup"><span data-stu-id="e49f4-206">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="e49f4-207">updateChannel</span><span class="sxs-lookup"><span data-stu-id="e49f4-207">updateChannel</span></span>|[<span data-ttu-id="e49f4-208">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="e49f4-208">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="e49f4-209">A propriedade para representar o canal de atualização Office365.</span><span class="sxs-lookup"><span data-stu-id="e49f4-209">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="e49f4-210">Os valores possíveis são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="e49f4-210">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="e49f4-211">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="e49f4-211">officePlatformArchitecture</span></span>|[<span data-ttu-id="e49f4-212">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e49f4-212">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e49f4-213">A propriedade para representar a versão do pacote de aplicativo Office365.</span><span class="sxs-lookup"><span data-stu-id="e49f4-213">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="e49f4-214">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="e49f4-214">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="e49f4-215">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="e49f4-215">localesToInstall</span></span>|<span data-ttu-id="e49f4-216">String collection</span><span class="sxs-lookup"><span data-stu-id="e49f4-216">String collection</span></span>|<span data-ttu-id="e49f4-217">A propriedade para representar as localidades que são instaladas quando os aplicativos a partir Office365 está instalado.</span><span class="sxs-lookup"><span data-stu-id="e49f4-217">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="e49f4-218">Ele usa 6033 standard do RFC.</span><span class="sxs-lookup"><span data-stu-id="e49f4-218">It uses standard RFC 6033.</span></span> <span data-ttu-id="e49f4-219">REF:https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="e49f4-219">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="e49f4-220">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="e49f4-220">installProgressDisplayLevel</span></span>|[<span data-ttu-id="e49f4-221">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="e49f4-221">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="e49f4-222">Para especificar o nível de exibição para a interface de usuário de instalação de progresso da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e49f4-222">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="e49f4-223">Os valores possíveis são: `none` e `full`.</span><span class="sxs-lookup"><span data-stu-id="e49f4-223">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="e49f4-224">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="e49f4-224">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="e49f4-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="e49f4-225">Boolean</span></span>|<span data-ttu-id="e49f4-226">A propriedade para determinar se você desinstalar o MSI existente do Office se um pacote do app Office365 é implantado com o dispositivo ou não.</span><span class="sxs-lookup"><span data-stu-id="e49f4-226">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="e49f4-227">targetVersion</span><span class="sxs-lookup"><span data-stu-id="e49f4-227">targetVersion</span></span>|<span data-ttu-id="e49f4-228">String</span><span class="sxs-lookup"><span data-stu-id="e49f4-228">String</span></span>|<span data-ttu-id="e49f4-229">A propriedade para representar a versão de destino específicos para o pacote do app Office365 que deve ser permaneceu implantada nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e49f4-229">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="e49f4-230">updateVersion</span><span class="sxs-lookup"><span data-stu-id="e49f4-230">updateVersion</span></span>|<span data-ttu-id="e49f4-231">String</span><span class="sxs-lookup"><span data-stu-id="e49f4-231">String</span></span>|<span data-ttu-id="e49f4-232">A propriedade para representar a versão de atualização em que a versão de destino específico está disponível para o pacote de aplicativo Office365.</span><span class="sxs-lookup"><span data-stu-id="e49f4-232">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|



## <a name="response"></a><span data-ttu-id="e49f4-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="e49f4-233">Response</span></span>
<span data-ttu-id="e49f4-234">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e49f4-234">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e49f4-235">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e49f4-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="e49f4-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e49f4-236">Request</span></span>
<span data-ttu-id="e49f4-237">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e49f4-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value"
}
```

### <a name="response"></a><span data-ttu-id="e49f4-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="e49f4-238">Response</span></span>
<span data-ttu-id="e49f4-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e49f4-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value"
}
```





