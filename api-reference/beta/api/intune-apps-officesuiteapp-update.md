---
title: Atualizar officeSuiteApp
description: Atualize as propriedades de um objeto officeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 24d5a8031580fa1d7cfe74415d84de32f49fa398
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979324"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="0bcf7-103">Atualizar officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="0bcf7-103">Update officeSuiteApp</span></span>

> <span data-ttu-id="0bcf7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bcf7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bcf7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bcf7-107">Atualize as propriedades de um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="0bcf7-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0bcf7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0bcf7-108">Prerequisites</span></span>
<span data-ttu-id="0bcf7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bcf7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bcf7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bcf7-111">Permission type</span></span>|<span data-ttu-id="0bcf7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bcf7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bcf7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bcf7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0bcf7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bcf7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-116">Not supported.</span></span>|
|<span data-ttu-id="0bcf7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bcf7-117">Application</span></span>|<span data-ttu-id="0bcf7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bcf7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bcf7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="0bcf7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bcf7-120">Request headers</span></span>
|<span data-ttu-id="0bcf7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0bcf7-121">Header</span></span>|<span data-ttu-id="0bcf7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0bcf7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bcf7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bcf7-123">Authorization</span></span>|<span data-ttu-id="0bcf7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bcf7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0bcf7-125">Accept</span></span>|<span data-ttu-id="0bcf7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bcf7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bcf7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bcf7-127">Request body</span></span>
<span data-ttu-id="0bcf7-128">No corpo da solicitação, fornece uma representação JSON para o objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="0bcf7-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="0bcf7-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="0bcf7-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="0bcf7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bcf7-130">Property</span></span>|<span data-ttu-id="0bcf7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bcf7-131">Type</span></span>|<span data-ttu-id="0bcf7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bcf7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bcf7-133">id</span><span class="sxs-lookup"><span data-stu-id="0bcf7-133">id</span></span>|<span data-ttu-id="0bcf7-134">String</span><span class="sxs-lookup"><span data-stu-id="0bcf7-134">String</span></span>|<span data-ttu-id="0bcf7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-135">Key of the entity.</span></span> <span data-ttu-id="0bcf7-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0bcf7-137">displayName</span></span>|<span data-ttu-id="0bcf7-138">String</span><span class="sxs-lookup"><span data-stu-id="0bcf7-138">String</span></span>|<span data-ttu-id="0bcf7-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0bcf7-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-141">description</span><span class="sxs-lookup"><span data-stu-id="0bcf7-141">description</span></span>|<span data-ttu-id="0bcf7-142">String</span><span class="sxs-lookup"><span data-stu-id="0bcf7-142">String</span></span>|<span data-ttu-id="0bcf7-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-143">The description of the app.</span></span> <span data-ttu-id="0bcf7-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="0bcf7-145">publisher</span></span>|<span data-ttu-id="0bcf7-146">String</span><span class="sxs-lookup"><span data-stu-id="0bcf7-146">String</span></span>|<span data-ttu-id="0bcf7-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-147">The publisher of the app.</span></span> <span data-ttu-id="0bcf7-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0bcf7-149">largeIcon</span></span>|[<span data-ttu-id="0bcf7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0bcf7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0bcf7-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0bcf7-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0bcf7-153">createdDateTime</span></span>|<span data-ttu-id="0bcf7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bcf7-154">DateTimeOffset</span></span>|<span data-ttu-id="0bcf7-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-155">The date and time the app was created.</span></span> <span data-ttu-id="0bcf7-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bcf7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="0bcf7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bcf7-158">DateTimeOffset</span></span>|<span data-ttu-id="0bcf7-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="0bcf7-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0bcf7-161">isFeatured</span></span>|<span data-ttu-id="0bcf7-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bcf7-162">Boolean</span></span>|<span data-ttu-id="0bcf7-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0bcf7-164">privacyInformationUrl</span></span>|<span data-ttu-id="0bcf7-165">String</span><span class="sxs-lookup"><span data-stu-id="0bcf7-165">String</span></span>|<span data-ttu-id="0bcf7-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-166">The privacy statement Url.</span></span> <span data-ttu-id="0bcf7-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0bcf7-168">informationUrl</span></span>|<span data-ttu-id="0bcf7-169">String</span><span class="sxs-lookup"><span data-stu-id="0bcf7-169">String</span></span>|<span data-ttu-id="0bcf7-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-170">The more information Url.</span></span> <span data-ttu-id="0bcf7-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-172">owner</span><span class="sxs-lookup"><span data-stu-id="0bcf7-172">owner</span></span>|<span data-ttu-id="0bcf7-173">String</span><span class="sxs-lookup"><span data-stu-id="0bcf7-173">String</span></span>|<span data-ttu-id="0bcf7-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-174">The owner of the app.</span></span> <span data-ttu-id="0bcf7-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-176">developer</span><span class="sxs-lookup"><span data-stu-id="0bcf7-176">developer</span></span>|<span data-ttu-id="0bcf7-177">String</span><span class="sxs-lookup"><span data-stu-id="0bcf7-177">String</span></span>|<span data-ttu-id="0bcf7-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-178">The developer of the app.</span></span> <span data-ttu-id="0bcf7-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-180">Observações</span><span class="sxs-lookup"><span data-stu-id="0bcf7-180">notes</span></span>|<span data-ttu-id="0bcf7-181">String</span><span class="sxs-lookup"><span data-stu-id="0bcf7-181">String</span></span>|<span data-ttu-id="0bcf7-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-182">Notes for the app.</span></span> <span data-ttu-id="0bcf7-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="0bcf7-184">uploadState</span></span>|<span data-ttu-id="0bcf7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0bcf7-185">Int32</span></span>|<span data-ttu-id="0bcf7-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-186">The upload state.</span></span> <span data-ttu-id="0bcf7-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0bcf7-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="0bcf7-188">publishingState</span></span>|[<span data-ttu-id="0bcf7-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0bcf7-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0bcf7-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-190">The publishing state for the app.</span></span> <span data-ttu-id="0bcf7-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0bcf7-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0bcf7-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0bcf7-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0bcf7-194">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="0bcf7-194">autoAcceptEula</span></span>|<span data-ttu-id="0bcf7-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bcf7-195">Boolean</span></span>|<span data-ttu-id="0bcf7-196">O valor para aceitar o EULA automaticamente no dispositivo do usuário final.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-196">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="0bcf7-197">productIds</span><span class="sxs-lookup"><span data-stu-id="0bcf7-197">productIds</span></span>|<span data-ttu-id="0bcf7-198">coleção [officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="0bcf7-198">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="0bcf7-199">As Ids de produto que representam a SKU do pacote Office365.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-199">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="0bcf7-200">Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-200">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="0bcf7-201">excludedApps</span><span class="sxs-lookup"><span data-stu-id="0bcf7-201">excludedApps</span></span>|[<span data-ttu-id="0bcf7-202">excludedApps</span><span class="sxs-lookup"><span data-stu-id="0bcf7-202">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="0bcf7-203">A propriedade para representar os aplicativos que são excluídos do produto selecionado Office365 ID.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-203">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="0bcf7-204">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="0bcf7-204">useSharedComputerActivation</span></span>|<span data-ttu-id="0bcf7-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bcf7-205">Boolean</span></span>|<span data-ttu-id="0bcf7-206">A propriedade para representar que se a ativação do computador compartilhado é usada não para o pacote do app Office365.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-206">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="0bcf7-207">updateChannel</span><span class="sxs-lookup"><span data-stu-id="0bcf7-207">updateChannel</span></span>|[<span data-ttu-id="0bcf7-208">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="0bcf7-208">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="0bcf7-209">A propriedade para representar o canal de atualização Office365.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-209">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="0bcf7-210">Os valores possíveis são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-210">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="0bcf7-211">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="0bcf7-211">officePlatformArchitecture</span></span>|[<span data-ttu-id="0bcf7-212">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="0bcf7-212">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="0bcf7-213">A propriedade para representar a versão do pacote de aplicativo Office365.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-213">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="0bcf7-214">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-214">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="0bcf7-215">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="0bcf7-215">localesToInstall</span></span>|<span data-ttu-id="0bcf7-216">String collection</span><span class="sxs-lookup"><span data-stu-id="0bcf7-216">String collection</span></span>|<span data-ttu-id="0bcf7-217">A propriedade para representar as localidades que são instaladas quando os aplicativos a partir Office365 está instalado.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-217">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="0bcf7-218">Ele usa 6033 standard do RFC.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-218">It uses standard RFC 6033.</span></span> <span data-ttu-id="0bcf7-219">REF:https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="0bcf7-219">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="0bcf7-220">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="0bcf7-220">installProgressDisplayLevel</span></span>|[<span data-ttu-id="0bcf7-221">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="0bcf7-221">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="0bcf7-222">Para especificar o nível de exibição para a interface de usuário de instalação de progresso da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-222">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="0bcf7-223">Os valores possíveis são: `none` e `full`.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-223">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="0bcf7-224">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="0bcf7-224">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="0bcf7-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bcf7-225">Boolean</span></span>|<span data-ttu-id="0bcf7-226">A propriedade para determinar se você desinstalar o MSI existente do Office se um pacote do app Office365 é implantado com o dispositivo ou não.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-226">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="0bcf7-227">targetVersion</span><span class="sxs-lookup"><span data-stu-id="0bcf7-227">targetVersion</span></span>|<span data-ttu-id="0bcf7-228">String</span><span class="sxs-lookup"><span data-stu-id="0bcf7-228">String</span></span>|<span data-ttu-id="0bcf7-229">A propriedade para representar a versão de destino específicos para o pacote do app Office365 que deve ser permaneceu implantada nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-229">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="0bcf7-230">updateVersion</span><span class="sxs-lookup"><span data-stu-id="0bcf7-230">updateVersion</span></span>|<span data-ttu-id="0bcf7-231">String</span><span class="sxs-lookup"><span data-stu-id="0bcf7-231">String</span></span>|<span data-ttu-id="0bcf7-232">A propriedade para representar a versão de atualização em que a versão de destino específico está disponível para o pacote de aplicativo Office365.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-232">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|



## <a name="response"></a><span data-ttu-id="0bcf7-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bcf7-233">Response</span></span>
<span data-ttu-id="0bcf7-234">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-234">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bcf7-235">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bcf7-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="0bcf7-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bcf7-236">Request</span></span>
<span data-ttu-id="0bcf7-237">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-237">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0bcf7-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bcf7-238">Response</span></span>
<span data-ttu-id="0bcf7-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bcf7-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





