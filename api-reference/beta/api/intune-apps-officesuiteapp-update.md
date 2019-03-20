---
title: Atualizar officeSuiteApp
description: Atualiza as propriedades de um objeto officeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6e8837741c7376d7f0c33740a0ed6420adf7c89
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572198"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="8eec7-103">Atualizar officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="8eec7-103">Update officeSuiteApp</span></span>

> <span data-ttu-id="8eec7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8eec7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8eec7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8eec7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eec7-106">Atualiza as propriedades de um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8eec7-106">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8eec7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8eec7-107">Prerequisites</span></span>
<span data-ttu-id="8eec7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8eec7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8eec7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8eec7-110">Permission type</span></span>|<span data-ttu-id="8eec7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8eec7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8eec7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8eec7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8eec7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eec7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8eec7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8eec7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8eec7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8eec7-115">Not supported.</span></span>|
|<span data-ttu-id="8eec7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8eec7-116">Application</span></span>|<span data-ttu-id="8eec7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8eec7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8eec7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8eec7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8eec7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8eec7-119">Request headers</span></span>
|<span data-ttu-id="8eec7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8eec7-120">Header</span></span>|<span data-ttu-id="8eec7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8eec7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8eec7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8eec7-122">Authorization</span></span>|<span data-ttu-id="8eec7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8eec7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8eec7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8eec7-124">Accept</span></span>|<span data-ttu-id="8eec7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8eec7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eec7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8eec7-126">Request body</span></span>
<span data-ttu-id="8eec7-127">No corpo da solicitação, forneça uma representação JSON do objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8eec7-127">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="8eec7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="8eec7-128">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="8eec7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8eec7-129">Property</span></span>|<span data-ttu-id="8eec7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8eec7-130">Type</span></span>|<span data-ttu-id="8eec7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8eec7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eec7-132">id</span><span class="sxs-lookup"><span data-stu-id="8eec7-132">id</span></span>|<span data-ttu-id="8eec7-133">String</span><span class="sxs-lookup"><span data-stu-id="8eec7-133">String</span></span>|<span data-ttu-id="8eec7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8eec7-134">Key of the entity.</span></span> <span data-ttu-id="8eec7-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8eec7-136">displayName</span></span>|<span data-ttu-id="8eec7-137">String</span><span class="sxs-lookup"><span data-stu-id="8eec7-137">String</span></span>|<span data-ttu-id="8eec7-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8eec7-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8eec7-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-140">descrição</span><span class="sxs-lookup"><span data-stu-id="8eec7-140">description</span></span>|<span data-ttu-id="8eec7-141">String</span><span class="sxs-lookup"><span data-stu-id="8eec7-141">String</span></span>|<span data-ttu-id="8eec7-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8eec7-142">The description of the app.</span></span> <span data-ttu-id="8eec7-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-144">publicador</span><span class="sxs-lookup"><span data-stu-id="8eec7-144">publisher</span></span>|<span data-ttu-id="8eec7-145">String</span><span class="sxs-lookup"><span data-stu-id="8eec7-145">String</span></span>|<span data-ttu-id="8eec7-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8eec7-146">The publisher of the app.</span></span> <span data-ttu-id="8eec7-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8eec7-148">largeIcon</span></span>|[<span data-ttu-id="8eec7-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8eec7-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8eec7-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8eec7-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8eec7-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8eec7-152">createdDateTime</span></span>|<span data-ttu-id="8eec7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eec7-153">DateTimeOffset</span></span>|<span data-ttu-id="8eec7-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8eec7-154">The date and time the app was created.</span></span> <span data-ttu-id="8eec7-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8eec7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="8eec7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eec7-157">DateTimeOffset</span></span>|<span data-ttu-id="8eec7-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8eec7-158">The date and time the app was last modified.</span></span> <span data-ttu-id="8eec7-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8eec7-160">isFeatured</span></span>|<span data-ttu-id="8eec7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eec7-161">Boolean</span></span>|<span data-ttu-id="8eec7-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8eec7-163">privacyInformationUrl</span></span>|<span data-ttu-id="8eec7-164">String</span><span class="sxs-lookup"><span data-stu-id="8eec7-164">String</span></span>|<span data-ttu-id="8eec7-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8eec7-165">The privacy statement Url.</span></span> <span data-ttu-id="8eec7-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8eec7-167">informationUrl</span></span>|<span data-ttu-id="8eec7-168">String</span><span class="sxs-lookup"><span data-stu-id="8eec7-168">String</span></span>|<span data-ttu-id="8eec7-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8eec7-169">The more information Url.</span></span> <span data-ttu-id="8eec7-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-171">owner</span><span class="sxs-lookup"><span data-stu-id="8eec7-171">owner</span></span>|<span data-ttu-id="8eec7-172">String</span><span class="sxs-lookup"><span data-stu-id="8eec7-172">String</span></span>|<span data-ttu-id="8eec7-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8eec7-173">The owner of the app.</span></span> <span data-ttu-id="8eec7-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-175">developer</span><span class="sxs-lookup"><span data-stu-id="8eec7-175">developer</span></span>|<span data-ttu-id="8eec7-176">String</span><span class="sxs-lookup"><span data-stu-id="8eec7-176">String</span></span>|<span data-ttu-id="8eec7-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8eec7-177">The developer of the app.</span></span> <span data-ttu-id="8eec7-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-179">notes</span><span class="sxs-lookup"><span data-stu-id="8eec7-179">notes</span></span>|<span data-ttu-id="8eec7-180">String</span><span class="sxs-lookup"><span data-stu-id="8eec7-180">String</span></span>|<span data-ttu-id="8eec7-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8eec7-181">Notes for the app.</span></span> <span data-ttu-id="8eec7-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="8eec7-183">uploadState</span></span>|<span data-ttu-id="8eec7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="8eec7-184">Int32</span></span>|<span data-ttu-id="8eec7-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="8eec7-185">The upload state.</span></span> <span data-ttu-id="8eec7-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="8eec7-187">publishingState</span></span>|[<span data-ttu-id="8eec7-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8eec7-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8eec7-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8eec7-189">The publishing state for the app.</span></span> <span data-ttu-id="8eec7-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8eec7-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8eec7-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8eec7-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8eec7-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8eec7-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8eec7-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8eec7-193">isAssigned</span></span>|<span data-ttu-id="8eec7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eec7-194">Boolean</span></span>|<span data-ttu-id="8eec7-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="8eec7-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8eec7-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8eec7-197">roleScopeTagIds</span></span>|<span data-ttu-id="8eec7-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eec7-198">String collection</span></span>|<span data-ttu-id="8eec7-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="8eec7-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8eec7-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8eec7-201">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="8eec7-201">autoAcceptEula</span></span>|<span data-ttu-id="8eec7-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eec7-202">Boolean</span></span>|<span data-ttu-id="8eec7-203">O valor para aceitar o EULA automaticamente no dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="8eec7-203">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="8eec7-204">productIds</span><span class="sxs-lookup"><span data-stu-id="8eec7-204">productIds</span></span>|<span data-ttu-id="8eec7-205">coleção [officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="8eec7-205">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="8eec7-206">As IDs de produto que representam a SKU do pacote do office365.</span><span class="sxs-lookup"><span data-stu-id="8eec7-206">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="8eec7-207">Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="8eec7-207">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="8eec7-208">excludedApps</span><span class="sxs-lookup"><span data-stu-id="8eec7-208">excludedApps</span></span>|[<span data-ttu-id="8eec7-209">excludedApps</span><span class="sxs-lookup"><span data-stu-id="8eec7-209">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="8eec7-210">A propriedade para representar os aplicativos que são excluídos da ID de produto do Office365 selecionado.</span><span class="sxs-lookup"><span data-stu-id="8eec7-210">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="8eec7-211">Propriedades usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="8eec7-211">useSharedComputerActivation</span></span>|<span data-ttu-id="8eec7-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eec7-212">Boolean</span></span>|<span data-ttu-id="8eec7-213">A propriedade que representa se a ativação de computador compartilhado é usada não para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="8eec7-213">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="8eec7-214">updateChannel</span><span class="sxs-lookup"><span data-stu-id="8eec7-214">updateChannel</span></span>|[<span data-ttu-id="8eec7-215">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="8eec7-215">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="8eec7-216">A propriedade para representar o canal de atualização do office365.</span><span class="sxs-lookup"><span data-stu-id="8eec7-216">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="8eec7-217">Os valores possíveis são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="8eec7-217">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="8eec7-218">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="8eec7-218">officePlatformArchitecture</span></span>|[<span data-ttu-id="8eec7-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="8eec7-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="8eec7-220">A propriedade para representar a versão do pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="8eec7-220">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="8eec7-221">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="8eec7-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="8eec7-222">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="8eec7-222">localesToInstall</span></span>|<span data-ttu-id="8eec7-223">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eec7-223">String collection</span></span>|<span data-ttu-id="8eec7-224">A propriedade para representar os locais que são instalados quando os aplicativos do Office365 estão instalados.</span><span class="sxs-lookup"><span data-stu-id="8eec7-224">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="8eec7-225">Ele usa RFC 6033 padrão.</span><span class="sxs-lookup"><span data-stu-id="8eec7-225">It uses standard RFC 6033.</span></span> <span data-ttu-id="8eec7-226">Refhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="8eec7-226">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="8eec7-227">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="8eec7-227">installProgressDisplayLevel</span></span>|[<span data-ttu-id="8eec7-228">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="8eec7-228">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="8eec7-229">Para especificar o nível de exibição da interface do usuário da configuração de progresso da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8eec7-229">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="8eec7-230">Os valores possíveis são: `none` e `full`.</span><span class="sxs-lookup"><span data-stu-id="8eec7-230">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="8eec7-231">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="8eec7-231">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="8eec7-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eec7-232">Boolean</span></span>|<span data-ttu-id="8eec7-233">A propriedade para determinar se deve desinstalar o Office MSI existente se um pacote de aplicativos do Office365 for implantado no dispositivo ou não.</span><span class="sxs-lookup"><span data-stu-id="8eec7-233">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="8eec7-234">targetVersion</span><span class="sxs-lookup"><span data-stu-id="8eec7-234">targetVersion</span></span>|<span data-ttu-id="8eec7-235">String</span><span class="sxs-lookup"><span data-stu-id="8eec7-235">String</span></span>|<span data-ttu-id="8eec7-236">A propriedade para representar a versão de destino específica para o pacote de aplicativos do Office365 que deve permanecer implantado nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8eec7-236">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="8eec7-237">updateVersion</span><span class="sxs-lookup"><span data-stu-id="8eec7-237">updateVersion</span></span>|<span data-ttu-id="8eec7-238">String</span><span class="sxs-lookup"><span data-stu-id="8eec7-238">String</span></span>|<span data-ttu-id="8eec7-239">A propriedade para representar a versão de atualização na qual a versão de destino específica está disponível para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="8eec7-239">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="8eec7-240">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="8eec7-240">officeConfigurationXml</span></span>|<span data-ttu-id="8eec7-241">Binário</span><span class="sxs-lookup"><span data-stu-id="8eec7-241">Binary</span></span>|<span data-ttu-id="8eec7-242">A propriedade para representar o arquivo de configuração XML que pode ser especificado para aplicativos do Office proPlus.</span><span class="sxs-lookup"><span data-stu-id="8eec7-242">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="8eec7-243">Tem precedência sobre todas as outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="8eec7-243">Takes precedence over all other properties.</span></span> <span data-ttu-id="8eec7-244">Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8eec7-244">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="8eec7-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="8eec7-245">Response</span></span>
<span data-ttu-id="8eec7-246">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8eec7-246">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eec7-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8eec7-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="8eec7-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8eec7-248">Request</span></span>
<span data-ttu-id="8eec7-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8eec7-249">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1572

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
    "teams": true,
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

### <a name="response"></a><span data-ttu-id="8eec7-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="8eec7-250">Response</span></span>
<span data-ttu-id="8eec7-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8eec7-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1744

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
    "teams": true,
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




