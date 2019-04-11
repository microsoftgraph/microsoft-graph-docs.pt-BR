---
title: Atualizar androidManagedStoreApp
description: Atualiza as propriedades de um objeto androidManagedStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5030ce96a61cb3f69ab2de5ab518cff3136d41c1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795916"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="bf9c6-103">Atualizar androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="bf9c6-103">Update androidManagedStoreApp</span></span>

> <span data-ttu-id="bf9c6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf9c6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf9c6-106">Atualiza as propriedades de um objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bf9c6-106">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf9c6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bf9c6-107">Prerequisites</span></span>
<span data-ttu-id="bf9c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf9c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf9c6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf9c6-110">Permission type</span></span>|<span data-ttu-id="bf9c6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf9c6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf9c6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf9c6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bf9c6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf9c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-115">Not supported.</span></span>|
|<span data-ttu-id="bf9c6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf9c6-116">Application</span></span>|<span data-ttu-id="bf9c6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf9c6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf9c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="bf9c6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf9c6-119">Request headers</span></span>
|<span data-ttu-id="bf9c6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bf9c6-120">Header</span></span>|<span data-ttu-id="bf9c6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bf9c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf9c6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf9c6-122">Authorization</span></span>|<span data-ttu-id="bf9c6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf9c6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bf9c6-124">Accept</span></span>|<span data-ttu-id="bf9c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf9c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf9c6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf9c6-126">Request body</span></span>
<span data-ttu-id="bf9c6-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bf9c6-127">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="bf9c6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="bf9c6-128">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="bf9c6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf9c6-129">Property</span></span>|<span data-ttu-id="bf9c6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf9c6-130">Type</span></span>|<span data-ttu-id="bf9c6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf9c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf9c6-132">id</span><span class="sxs-lookup"><span data-stu-id="bf9c6-132">id</span></span>|<span data-ttu-id="bf9c6-133">String</span><span class="sxs-lookup"><span data-stu-id="bf9c6-133">String</span></span>|<span data-ttu-id="bf9c6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-134">Key of the entity.</span></span> <span data-ttu-id="bf9c6-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bf9c6-136">displayName</span></span>|<span data-ttu-id="bf9c6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf9c6-137">String</span></span>|<span data-ttu-id="bf9c6-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bf9c6-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-140">description</span><span class="sxs-lookup"><span data-stu-id="bf9c6-140">description</span></span>|<span data-ttu-id="bf9c6-141">String</span><span class="sxs-lookup"><span data-stu-id="bf9c6-141">String</span></span>|<span data-ttu-id="bf9c6-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-142">The description of the app.</span></span> <span data-ttu-id="bf9c6-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-144">publicador</span><span class="sxs-lookup"><span data-stu-id="bf9c6-144">publisher</span></span>|<span data-ttu-id="bf9c6-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf9c6-145">String</span></span>|<span data-ttu-id="bf9c6-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-146">The publisher of the app.</span></span> <span data-ttu-id="bf9c6-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bf9c6-148">largeIcon</span></span>|[<span data-ttu-id="bf9c6-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bf9c6-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bf9c6-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bf9c6-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf9c6-152">createdDateTime</span></span>|<span data-ttu-id="bf9c6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf9c6-153">DateTimeOffset</span></span>|<span data-ttu-id="bf9c6-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-154">The date and time the app was created.</span></span> <span data-ttu-id="bf9c6-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf9c6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="bf9c6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf9c6-157">DateTimeOffset</span></span>|<span data-ttu-id="bf9c6-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-158">The date and time the app was last modified.</span></span> <span data-ttu-id="bf9c6-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bf9c6-160">isFeatured</span></span>|<span data-ttu-id="bf9c6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf9c6-161">Boolean</span></span>|<span data-ttu-id="bf9c6-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bf9c6-163">privacyInformationUrl</span></span>|<span data-ttu-id="bf9c6-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf9c6-164">String</span></span>|<span data-ttu-id="bf9c6-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-165">The privacy statement Url.</span></span> <span data-ttu-id="bf9c6-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bf9c6-167">informationUrl</span></span>|<span data-ttu-id="bf9c6-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf9c6-168">String</span></span>|<span data-ttu-id="bf9c6-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-169">The more information Url.</span></span> <span data-ttu-id="bf9c6-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-171">owner</span><span class="sxs-lookup"><span data-stu-id="bf9c6-171">owner</span></span>|<span data-ttu-id="bf9c6-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf9c6-172">String</span></span>|<span data-ttu-id="bf9c6-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-173">The owner of the app.</span></span> <span data-ttu-id="bf9c6-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-175">developer</span><span class="sxs-lookup"><span data-stu-id="bf9c6-175">developer</span></span>|<span data-ttu-id="bf9c6-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf9c6-176">String</span></span>|<span data-ttu-id="bf9c6-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-177">The developer of the app.</span></span> <span data-ttu-id="bf9c6-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-179">notes</span><span class="sxs-lookup"><span data-stu-id="bf9c6-179">notes</span></span>|<span data-ttu-id="bf9c6-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf9c6-180">String</span></span>|<span data-ttu-id="bf9c6-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-181">Notes for the app.</span></span> <span data-ttu-id="bf9c6-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="bf9c6-183">uploadState</span></span>|<span data-ttu-id="bf9c6-184">Int32</span><span class="sxs-lookup"><span data-stu-id="bf9c6-184">Int32</span></span>|<span data-ttu-id="bf9c6-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-185">The upload state.</span></span> <span data-ttu-id="bf9c6-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="bf9c6-187">publishingState</span></span>|[<span data-ttu-id="bf9c6-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bf9c6-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bf9c6-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-189">The publishing state for the app.</span></span> <span data-ttu-id="bf9c6-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bf9c6-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bf9c6-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="bf9c6-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bf9c6-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bf9c6-193">isAssigned</span></span>|<span data-ttu-id="bf9c6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf9c6-194">Boolean</span></span>|<span data-ttu-id="bf9c6-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="bf9c6-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bf9c6-197">roleScopeTagIds</span></span>|<span data-ttu-id="bf9c6-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="bf9c6-198">String collection</span></span>|<span data-ttu-id="bf9c6-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="bf9c6-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="bf9c6-201">dependentAppCount</span></span>|<span data-ttu-id="bf9c6-202">Int32</span><span class="sxs-lookup"><span data-stu-id="bf9c6-202">Int32</span></span>|<span data-ttu-id="bf9c6-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="bf9c6-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf9c6-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf9c6-205">packageId</span><span class="sxs-lookup"><span data-stu-id="bf9c6-205">packageId</span></span>|<span data-ttu-id="bf9c6-206">String</span><span class="sxs-lookup"><span data-stu-id="bf9c6-206">String</span></span>|<span data-ttu-id="bf9c6-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-207">The package identifier.</span></span>|
|<span data-ttu-id="bf9c6-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="bf9c6-208">appIdentifier</span></span>|<span data-ttu-id="bf9c6-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf9c6-209">String</span></span>|<span data-ttu-id="bf9c6-210">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-210">The Identity Name.</span></span>|
|<span data-ttu-id="bf9c6-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="bf9c6-211">usedLicenseCount</span></span>|<span data-ttu-id="bf9c6-212">Int32</span><span class="sxs-lookup"><span data-stu-id="bf9c6-212">Int32</span></span>|<span data-ttu-id="bf9c6-213">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="bf9c6-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="bf9c6-214">totalLicenseCount</span></span>|<span data-ttu-id="bf9c6-215">Int32</span><span class="sxs-lookup"><span data-stu-id="bf9c6-215">Int32</span></span>|<span data-ttu-id="bf9c6-216">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="bf9c6-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="bf9c6-217">appStoreUrl</span></span>|<span data-ttu-id="bf9c6-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf9c6-218">String</span></span>|<span data-ttu-id="bf9c6-219">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-219">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="bf9c6-220">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="bf9c6-220">supportsOemConfig</span></span>|<span data-ttu-id="bf9c6-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf9c6-221">Boolean</span></span>|<span data-ttu-id="bf9c6-222">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-222">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="bf9c6-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf9c6-223">Response</span></span>
<span data-ttu-id="bf9c6-224">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-224">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf9c6-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf9c6-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf9c6-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf9c6-226">Request</span></span>
<span data-ttu-id="bf9c6-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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
  "dependentAppCount": 1,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="bf9c6-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf9c6-228">Response</span></span>
<span data-ttu-id="bf9c6-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf9c6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "dependentAppCount": 1,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```





