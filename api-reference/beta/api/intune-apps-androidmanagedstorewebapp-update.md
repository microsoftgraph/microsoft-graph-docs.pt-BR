---
title: Atualizar androidManagedStoreWebApp
description: Atualiza as propriedades de um objeto androidManagedStoreWebApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6cbc3dee0f59f1c4b534fb5fd9747473801d7a66
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39926275"
---
# <a name="update-androidmanagedstorewebapp"></a><span data-ttu-id="96f42-103">Atualizar androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="96f42-103">Update androidManagedStoreWebApp</span></span>

> <span data-ttu-id="96f42-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96f42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96f42-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96f42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96f42-106">Atualiza as propriedades de um objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="96f42-106">Update the properties of a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96f42-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96f42-107">Prerequisites</span></span>
<span data-ttu-id="96f42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96f42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96f42-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96f42-110">Permission type</span></span>|<span data-ttu-id="96f42-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96f42-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96f42-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96f42-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96f42-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96f42-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96f42-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96f42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96f42-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96f42-115">Not supported.</span></span>|
|<span data-ttu-id="96f42-116">Application</span><span class="sxs-lookup"><span data-stu-id="96f42-116">Application</span></span>|<span data-ttu-id="96f42-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96f42-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96f42-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96f42-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="96f42-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96f42-119">Request headers</span></span>
|<span data-ttu-id="96f42-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96f42-120">Header</span></span>|<span data-ttu-id="96f42-121">Valor</span><span class="sxs-lookup"><span data-stu-id="96f42-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96f42-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="96f42-122">Authorization</span></span>|<span data-ttu-id="96f42-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96f42-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96f42-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96f42-124">Accept</span></span>|<span data-ttu-id="96f42-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96f42-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96f42-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96f42-126">Request body</span></span>
<span data-ttu-id="96f42-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="96f42-127">In the request body, supply a JSON representation for the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

<span data-ttu-id="96f42-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span><span class="sxs-lookup"><span data-stu-id="96f42-128">The following table shows the properties that are required when you create the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

|<span data-ttu-id="96f42-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96f42-129">Property</span></span>|<span data-ttu-id="96f42-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="96f42-130">Type</span></span>|<span data-ttu-id="96f42-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="96f42-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96f42-132">id</span><span class="sxs-lookup"><span data-stu-id="96f42-132">id</span></span>|<span data-ttu-id="96f42-133">String</span><span class="sxs-lookup"><span data-stu-id="96f42-133">String</span></span>|<span data-ttu-id="96f42-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="96f42-134">Key of the entity.</span></span> <span data-ttu-id="96f42-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-136">displayName</span><span class="sxs-lookup"><span data-stu-id="96f42-136">displayName</span></span>|<span data-ttu-id="96f42-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96f42-137">String</span></span>|<span data-ttu-id="96f42-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="96f42-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="96f42-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-140">description</span><span class="sxs-lookup"><span data-stu-id="96f42-140">description</span></span>|<span data-ttu-id="96f42-141">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="96f42-141">String</span></span>|<span data-ttu-id="96f42-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96f42-142">The description of the app.</span></span> <span data-ttu-id="96f42-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-144">publicador</span><span class="sxs-lookup"><span data-stu-id="96f42-144">publisher</span></span>|<span data-ttu-id="96f42-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="96f42-145">String</span></span>|<span data-ttu-id="96f42-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96f42-146">The publisher of the app.</span></span> <span data-ttu-id="96f42-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="96f42-148">largeIcon</span></span>|[<span data-ttu-id="96f42-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="96f42-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="96f42-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="96f42-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="96f42-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96f42-152">createdDateTime</span></span>|<span data-ttu-id="96f42-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96f42-153">DateTimeOffset</span></span>|<span data-ttu-id="96f42-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96f42-154">The date and time the app was created.</span></span> <span data-ttu-id="96f42-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96f42-156">lastModifiedDateTime</span></span>|<span data-ttu-id="96f42-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96f42-157">DateTimeOffset</span></span>|<span data-ttu-id="96f42-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="96f42-158">The date and time the app was last modified.</span></span> <span data-ttu-id="96f42-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="96f42-160">isFeatured</span></span>|<span data-ttu-id="96f42-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="96f42-161">Boolean</span></span>|<span data-ttu-id="96f42-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="96f42-163">privacyInformationUrl</span></span>|<span data-ttu-id="96f42-164">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="96f42-164">String</span></span>|<span data-ttu-id="96f42-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="96f42-165">The privacy statement Url.</span></span> <span data-ttu-id="96f42-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="96f42-167">informationUrl</span></span>|<span data-ttu-id="96f42-168">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="96f42-168">String</span></span>|<span data-ttu-id="96f42-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="96f42-169">The more information Url.</span></span> <span data-ttu-id="96f42-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-171">owner</span><span class="sxs-lookup"><span data-stu-id="96f42-171">owner</span></span>|<span data-ttu-id="96f42-172">String</span><span class="sxs-lookup"><span data-stu-id="96f42-172">String</span></span>|<span data-ttu-id="96f42-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="96f42-173">The owner of the app.</span></span> <span data-ttu-id="96f42-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-175">developer</span><span class="sxs-lookup"><span data-stu-id="96f42-175">developer</span></span>|<span data-ttu-id="96f42-176">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="96f42-176">String</span></span>|<span data-ttu-id="96f42-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96f42-177">The developer of the app.</span></span> <span data-ttu-id="96f42-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-179">notes</span><span class="sxs-lookup"><span data-stu-id="96f42-179">notes</span></span>|<span data-ttu-id="96f42-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="96f42-180">String</span></span>|<span data-ttu-id="96f42-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96f42-181">Notes for the app.</span></span> <span data-ttu-id="96f42-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="96f42-183">uploadState</span></span>|<span data-ttu-id="96f42-184">Int32</span><span class="sxs-lookup"><span data-stu-id="96f42-184">Int32</span></span>|<span data-ttu-id="96f42-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="96f42-185">The upload state.</span></span> <span data-ttu-id="96f42-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="96f42-187">publishingState</span></span>|[<span data-ttu-id="96f42-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="96f42-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="96f42-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96f42-189">The publishing state for the app.</span></span> <span data-ttu-id="96f42-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="96f42-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="96f42-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96f42-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="96f42-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="96f42-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="96f42-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="96f42-193">isAssigned</span></span>|<span data-ttu-id="96f42-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="96f42-194">Boolean</span></span>|<span data-ttu-id="96f42-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="96f42-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="96f42-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="96f42-197">roleScopeTagIds</span></span>|<span data-ttu-id="96f42-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="96f42-198">String collection</span></span>|<span data-ttu-id="96f42-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="96f42-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="96f42-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="96f42-201">dependentAppCount</span></span>|<span data-ttu-id="96f42-202">Int32</span><span class="sxs-lookup"><span data-stu-id="96f42-202">Int32</span></span>|<span data-ttu-id="96f42-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="96f42-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="96f42-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96f42-205">packageId</span><span class="sxs-lookup"><span data-stu-id="96f42-205">packageId</span></span>|<span data-ttu-id="96f42-206">String</span><span class="sxs-lookup"><span data-stu-id="96f42-206">String</span></span>|<span data-ttu-id="96f42-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="96f42-207">The package identifier.</span></span> <span data-ttu-id="96f42-208">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-208">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="96f42-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="96f42-209">appIdentifier</span></span>|<span data-ttu-id="96f42-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96f42-210">String</span></span>|<span data-ttu-id="96f42-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="96f42-211">The Identity Name.</span></span> <span data-ttu-id="96f42-212">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-212">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="96f42-213">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="96f42-213">usedLicenseCount</span></span>|<span data-ttu-id="96f42-214">Int32</span><span class="sxs-lookup"><span data-stu-id="96f42-214">Int32</span></span>|<span data-ttu-id="96f42-215">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="96f42-215">The number of VPP licenses in use.</span></span> <span data-ttu-id="96f42-216">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-216">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="96f42-217">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="96f42-217">totalLicenseCount</span></span>|<span data-ttu-id="96f42-218">Int32</span><span class="sxs-lookup"><span data-stu-id="96f42-218">Int32</span></span>|<span data-ttu-id="96f42-219">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="96f42-219">The total number of VPP licenses.</span></span> <span data-ttu-id="96f42-220">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-220">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="96f42-221">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="96f42-221">appStoreUrl</span></span>|<span data-ttu-id="96f42-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96f42-222">String</span></span>|<span data-ttu-id="96f42-223">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="96f42-223">The Play for Work Store app URL.</span></span> <span data-ttu-id="96f42-224">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-224">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="96f42-225">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="96f42-225">isPrivate</span></span>|<span data-ttu-id="96f42-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="96f42-226">Boolean</span></span>|<span data-ttu-id="96f42-227">Indica se o aplicativo está disponível somente para os usuários de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="96f42-227">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="96f42-228">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-228">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="96f42-229">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="96f42-229">isSystemApp</span></span>|<span data-ttu-id="96f42-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="96f42-230">Boolean</span></span>|<span data-ttu-id="96f42-231">Indica se o aplicativo é um aplicativo de sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="96f42-231">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="96f42-232">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-232">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="96f42-233">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="96f42-233">supportsOemConfig</span></span>|<span data-ttu-id="96f42-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="96f42-234">Boolean</span></span>|<span data-ttu-id="96f42-235">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="96f42-235">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="96f42-236">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="96f42-236">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="96f42-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="96f42-237">Response</span></span>
<span data-ttu-id="96f42-238">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96f42-238">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96f42-239">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96f42-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="96f42-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96f42-240">Request</span></span>
<span data-ttu-id="96f42-241">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96f42-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 987

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="96f42-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="96f42-242">Response</span></span>
<span data-ttu-id="96f42-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96f42-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1159

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
  "id": "e54aecbd-ecbd-e54a-bdec-4ae5bdec4ae5",
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
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```





