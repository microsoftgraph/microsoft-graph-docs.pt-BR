---
title: Atualizar officeSuiteApp
description: Atualize as propriedades de um objeto officeSuiteApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a6b286c53cfcd6d6b93a91ea63cb1e693e168e57
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405314"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="15329-103">Atualizar officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="15329-103">Update officeSuiteApp</span></span>

> <span data-ttu-id="15329-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="15329-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15329-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="15329-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15329-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="15329-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15329-107">Atualize as propriedades de um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="15329-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15329-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15329-108">Prerequisites</span></span>
<span data-ttu-id="15329-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="15329-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15329-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15329-111">Permission type</span></span>|<span data-ttu-id="15329-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15329-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15329-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15329-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15329-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15329-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="15329-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15329-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15329-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15329-116">Not supported.</span></span>|
|<span data-ttu-id="15329-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15329-117">Application</span></span>|<span data-ttu-id="15329-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15329-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15329-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15329-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="15329-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15329-120">Request headers</span></span>
|<span data-ttu-id="15329-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15329-121">Header</span></span>|<span data-ttu-id="15329-122">Valor</span><span class="sxs-lookup"><span data-stu-id="15329-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15329-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="15329-123">Authorization</span></span>|<span data-ttu-id="15329-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15329-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15329-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15329-125">Accept</span></span>|<span data-ttu-id="15329-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15329-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15329-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15329-127">Request body</span></span>
<span data-ttu-id="15329-128">No corpo da solicitação, fornece uma representação JSON para o objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="15329-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="15329-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="15329-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="15329-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15329-130">Property</span></span>|<span data-ttu-id="15329-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="15329-131">Type</span></span>|<span data-ttu-id="15329-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="15329-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15329-133">id</span><span class="sxs-lookup"><span data-stu-id="15329-133">id</span></span>|<span data-ttu-id="15329-134">String</span><span class="sxs-lookup"><span data-stu-id="15329-134">String</span></span>|<span data-ttu-id="15329-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="15329-135">Key of the entity.</span></span> <span data-ttu-id="15329-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-137">displayName</span><span class="sxs-lookup"><span data-stu-id="15329-137">displayName</span></span>|<span data-ttu-id="15329-138">String</span><span class="sxs-lookup"><span data-stu-id="15329-138">String</span></span>|<span data-ttu-id="15329-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="15329-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="15329-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-141">description</span><span class="sxs-lookup"><span data-stu-id="15329-141">description</span></span>|<span data-ttu-id="15329-142">String</span><span class="sxs-lookup"><span data-stu-id="15329-142">String</span></span>|<span data-ttu-id="15329-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15329-143">The description of the app.</span></span> <span data-ttu-id="15329-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-145">publisher</span><span class="sxs-lookup"><span data-stu-id="15329-145">publisher</span></span>|<span data-ttu-id="15329-146">String</span><span class="sxs-lookup"><span data-stu-id="15329-146">String</span></span>|<span data-ttu-id="15329-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15329-147">The publisher of the app.</span></span> <span data-ttu-id="15329-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="15329-149">largeIcon</span></span>|[<span data-ttu-id="15329-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="15329-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="15329-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="15329-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="15329-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15329-153">createdDateTime</span></span>|<span data-ttu-id="15329-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15329-154">DateTimeOffset</span></span>|<span data-ttu-id="15329-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15329-155">The date and time the app was created.</span></span> <span data-ttu-id="15329-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15329-157">lastModifiedDateTime</span></span>|<span data-ttu-id="15329-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15329-158">DateTimeOffset</span></span>|<span data-ttu-id="15329-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="15329-159">The date and time the app was last modified.</span></span> <span data-ttu-id="15329-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="15329-161">isFeatured</span></span>|<span data-ttu-id="15329-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="15329-162">Boolean</span></span>|<span data-ttu-id="15329-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="15329-164">privacyInformationUrl</span></span>|<span data-ttu-id="15329-165">String</span><span class="sxs-lookup"><span data-stu-id="15329-165">String</span></span>|<span data-ttu-id="15329-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="15329-166">The privacy statement Url.</span></span> <span data-ttu-id="15329-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="15329-168">informationUrl</span></span>|<span data-ttu-id="15329-169">String</span><span class="sxs-lookup"><span data-stu-id="15329-169">String</span></span>|<span data-ttu-id="15329-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="15329-170">The more information Url.</span></span> <span data-ttu-id="15329-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-172">owner</span><span class="sxs-lookup"><span data-stu-id="15329-172">owner</span></span>|<span data-ttu-id="15329-173">String</span><span class="sxs-lookup"><span data-stu-id="15329-173">String</span></span>|<span data-ttu-id="15329-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="15329-174">The owner of the app.</span></span> <span data-ttu-id="15329-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-176">developer</span><span class="sxs-lookup"><span data-stu-id="15329-176">developer</span></span>|<span data-ttu-id="15329-177">String</span><span class="sxs-lookup"><span data-stu-id="15329-177">String</span></span>|<span data-ttu-id="15329-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15329-178">The developer of the app.</span></span> <span data-ttu-id="15329-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-180">Observações</span><span class="sxs-lookup"><span data-stu-id="15329-180">notes</span></span>|<span data-ttu-id="15329-181">String</span><span class="sxs-lookup"><span data-stu-id="15329-181">String</span></span>|<span data-ttu-id="15329-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15329-182">Notes for the app.</span></span> <span data-ttu-id="15329-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="15329-184">uploadState</span></span>|<span data-ttu-id="15329-185">Int32</span><span class="sxs-lookup"><span data-stu-id="15329-185">Int32</span></span>|<span data-ttu-id="15329-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="15329-186">The upload state.</span></span> <span data-ttu-id="15329-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="15329-188">publishingState</span></span>|[<span data-ttu-id="15329-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="15329-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="15329-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15329-190">The publishing state for the app.</span></span> <span data-ttu-id="15329-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="15329-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="15329-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="15329-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="15329-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="15329-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="15329-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="15329-194">isAssigned</span></span>|<span data-ttu-id="15329-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="15329-195">Boolean</span></span>|<span data-ttu-id="15329-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="15329-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="15329-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15329-198">roleScopeTagIds</span></span>|<span data-ttu-id="15329-199">String collection</span><span class="sxs-lookup"><span data-stu-id="15329-199">String collection</span></span>|<span data-ttu-id="15329-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="15329-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="15329-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15329-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15329-202">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="15329-202">autoAcceptEula</span></span>|<span data-ttu-id="15329-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="15329-203">Boolean</span></span>|<span data-ttu-id="15329-204">O valor para aceitar o EULA automaticamente no dispositivo do usuário final.</span><span class="sxs-lookup"><span data-stu-id="15329-204">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="15329-205">productIds</span><span class="sxs-lookup"><span data-stu-id="15329-205">productIds</span></span>|<span data-ttu-id="15329-206">coleção [officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="15329-206">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="15329-207">As Ids de produto que representam a SKU do pacote Office365.</span><span class="sxs-lookup"><span data-stu-id="15329-207">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="15329-208">Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="15329-208">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="15329-209">excludedApps</span><span class="sxs-lookup"><span data-stu-id="15329-209">excludedApps</span></span>|[<span data-ttu-id="15329-210">excludedApps</span><span class="sxs-lookup"><span data-stu-id="15329-210">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="15329-211">A propriedade para representar os aplicativos que são excluídos do produto selecionado Office365 ID.</span><span class="sxs-lookup"><span data-stu-id="15329-211">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="15329-212">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="15329-212">useSharedComputerActivation</span></span>|<span data-ttu-id="15329-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="15329-213">Boolean</span></span>|<span data-ttu-id="15329-214">A propriedade para representar que se a ativação do computador compartilhado é usada não para o pacote do app Office365.</span><span class="sxs-lookup"><span data-stu-id="15329-214">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="15329-215">updateChannel</span><span class="sxs-lookup"><span data-stu-id="15329-215">updateChannel</span></span>|[<span data-ttu-id="15329-216">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="15329-216">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="15329-217">A propriedade para representar o canal de atualização Office365.</span><span class="sxs-lookup"><span data-stu-id="15329-217">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="15329-218">Os valores possíveis são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="15329-218">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="15329-219">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="15329-219">officePlatformArchitecture</span></span>|[<span data-ttu-id="15329-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="15329-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="15329-221">A propriedade para representar a versão do pacote de aplicativo Office365.</span><span class="sxs-lookup"><span data-stu-id="15329-221">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="15329-222">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="15329-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="15329-223">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="15329-223">localesToInstall</span></span>|<span data-ttu-id="15329-224">String collection</span><span class="sxs-lookup"><span data-stu-id="15329-224">String collection</span></span>|<span data-ttu-id="15329-225">A propriedade para representar as localidades que são instaladas quando os aplicativos a partir Office365 está instalado.</span><span class="sxs-lookup"><span data-stu-id="15329-225">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="15329-226">Ele usa 6033 standard do RFC.</span><span class="sxs-lookup"><span data-stu-id="15329-226">It uses standard RFC 6033.</span></span> <span data-ttu-id="15329-227">REF:https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="15329-227">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="15329-228">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="15329-228">installProgressDisplayLevel</span></span>|[<span data-ttu-id="15329-229">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="15329-229">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="15329-230">Para especificar o nível de exibição para a interface de usuário de instalação de progresso da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15329-230">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="15329-231">Os valores possíveis são: `none` e `full`.</span><span class="sxs-lookup"><span data-stu-id="15329-231">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="15329-232">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="15329-232">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="15329-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="15329-233">Boolean</span></span>|<span data-ttu-id="15329-234">A propriedade para determinar se você desinstalar o MSI existente do Office se um pacote do app Office365 é implantado com o dispositivo ou não.</span><span class="sxs-lookup"><span data-stu-id="15329-234">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="15329-235">targetVersion</span><span class="sxs-lookup"><span data-stu-id="15329-235">targetVersion</span></span>|<span data-ttu-id="15329-236">String</span><span class="sxs-lookup"><span data-stu-id="15329-236">String</span></span>|<span data-ttu-id="15329-237">A propriedade para representar a versão de destino específicos para o pacote do app Office365 que deve ser permaneceu implantada nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="15329-237">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="15329-238">updateVersion</span><span class="sxs-lookup"><span data-stu-id="15329-238">updateVersion</span></span>|<span data-ttu-id="15329-239">String</span><span class="sxs-lookup"><span data-stu-id="15329-239">String</span></span>|<span data-ttu-id="15329-240">A propriedade para representar a versão de atualização em que a versão de destino específico está disponível para o pacote de aplicativo Office365.</span><span class="sxs-lookup"><span data-stu-id="15329-240">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="15329-241">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="15329-241">officeConfigurationXml</span></span>|<span data-ttu-id="15329-242">Binária</span><span class="sxs-lookup"><span data-stu-id="15329-242">Binary</span></span>|<span data-ttu-id="15329-243">A propriedade para representar o arquivo de configuração XML que pode ser especificado para o Office ProPlus Apps.</span><span class="sxs-lookup"><span data-stu-id="15329-243">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="15329-244">Tem precedência sobre todas as outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="15329-244">Takes precedence over all other properties.</span></span> <span data-ttu-id="15329-245">Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15329-245">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="15329-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="15329-246">Response</span></span>
<span data-ttu-id="15329-247">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15329-247">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15329-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15329-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="15329-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15329-249">Request</span></span>
<span data-ttu-id="15329-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15329-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1552

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="15329-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="15329-251">Response</span></span>
<span data-ttu-id="15329-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15329-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1724

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```




