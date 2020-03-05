---
title: Atualizar androidManagedStoreApp
description: Atualiza as propriedades de um objeto androidManagedStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8cf1e898e64ec2b8d958d935372553f8ca91993
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445894"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="eec28-103">Atualizar androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="eec28-103">Update androidManagedStoreApp</span></span>

<span data-ttu-id="eec28-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eec28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eec28-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eec28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eec28-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eec28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eec28-107">Atualiza as propriedades de um objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="eec28-107">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eec28-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eec28-108">Prerequisites</span></span>
<span data-ttu-id="eec28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eec28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eec28-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eec28-111">Permission type</span></span>|<span data-ttu-id="eec28-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eec28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eec28-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eec28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eec28-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eec28-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eec28-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eec28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eec28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eec28-116">Not supported.</span></span>|
|<span data-ttu-id="eec28-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eec28-117">Application</span></span>|<span data-ttu-id="eec28-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eec28-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eec28-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eec28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="eec28-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eec28-120">Request headers</span></span>
|<span data-ttu-id="eec28-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eec28-121">Header</span></span>|<span data-ttu-id="eec28-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eec28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eec28-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eec28-123">Authorization</span></span>|<span data-ttu-id="eec28-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eec28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eec28-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eec28-125">Accept</span></span>|<span data-ttu-id="eec28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eec28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eec28-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eec28-127">Request body</span></span>
<span data-ttu-id="eec28-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="eec28-128">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="eec28-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="eec28-129">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="eec28-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eec28-130">Property</span></span>|<span data-ttu-id="eec28-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="eec28-131">Type</span></span>|<span data-ttu-id="eec28-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="eec28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eec28-133">id</span><span class="sxs-lookup"><span data-stu-id="eec28-133">id</span></span>|<span data-ttu-id="eec28-134">String</span><span class="sxs-lookup"><span data-stu-id="eec28-134">String</span></span>|<span data-ttu-id="eec28-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="eec28-135">Key of the entity.</span></span> <span data-ttu-id="eec28-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-137">displayName</span><span class="sxs-lookup"><span data-stu-id="eec28-137">displayName</span></span>|<span data-ttu-id="eec28-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eec28-138">String</span></span>|<span data-ttu-id="eec28-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="eec28-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="eec28-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-141">description</span><span class="sxs-lookup"><span data-stu-id="eec28-141">description</span></span>|<span data-ttu-id="eec28-142">String</span><span class="sxs-lookup"><span data-stu-id="eec28-142">String</span></span>|<span data-ttu-id="eec28-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eec28-143">The description of the app.</span></span> <span data-ttu-id="eec28-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-145">publicador</span><span class="sxs-lookup"><span data-stu-id="eec28-145">publisher</span></span>|<span data-ttu-id="eec28-146">String</span><span class="sxs-lookup"><span data-stu-id="eec28-146">String</span></span>|<span data-ttu-id="eec28-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eec28-147">The publisher of the app.</span></span> <span data-ttu-id="eec28-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eec28-149">largeIcon</span></span>|[<span data-ttu-id="eec28-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eec28-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eec28-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="eec28-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="eec28-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eec28-153">createdDateTime</span></span>|<span data-ttu-id="eec28-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eec28-154">DateTimeOffset</span></span>|<span data-ttu-id="eec28-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eec28-155">The date and time the app was created.</span></span> <span data-ttu-id="eec28-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eec28-157">lastModifiedDateTime</span></span>|<span data-ttu-id="eec28-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eec28-158">DateTimeOffset</span></span>|<span data-ttu-id="eec28-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="eec28-159">The date and time the app was last modified.</span></span> <span data-ttu-id="eec28-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eec28-161">isFeatured</span></span>|<span data-ttu-id="eec28-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="eec28-162">Boolean</span></span>|<span data-ttu-id="eec28-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eec28-164">privacyInformationUrl</span></span>|<span data-ttu-id="eec28-165">String</span><span class="sxs-lookup"><span data-stu-id="eec28-165">String</span></span>|<span data-ttu-id="eec28-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="eec28-166">The privacy statement Url.</span></span> <span data-ttu-id="eec28-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eec28-168">informationUrl</span></span>|<span data-ttu-id="eec28-169">String</span><span class="sxs-lookup"><span data-stu-id="eec28-169">String</span></span>|<span data-ttu-id="eec28-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="eec28-170">The more information Url.</span></span> <span data-ttu-id="eec28-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-172">owner</span><span class="sxs-lookup"><span data-stu-id="eec28-172">owner</span></span>|<span data-ttu-id="eec28-173">String</span><span class="sxs-lookup"><span data-stu-id="eec28-173">String</span></span>|<span data-ttu-id="eec28-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="eec28-174">The owner of the app.</span></span> <span data-ttu-id="eec28-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-176">developer</span><span class="sxs-lookup"><span data-stu-id="eec28-176">developer</span></span>|<span data-ttu-id="eec28-177">String</span><span class="sxs-lookup"><span data-stu-id="eec28-177">String</span></span>|<span data-ttu-id="eec28-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eec28-178">The developer of the app.</span></span> <span data-ttu-id="eec28-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-180">notes</span><span class="sxs-lookup"><span data-stu-id="eec28-180">notes</span></span>|<span data-ttu-id="eec28-181">String</span><span class="sxs-lookup"><span data-stu-id="eec28-181">String</span></span>|<span data-ttu-id="eec28-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eec28-182">Notes for the app.</span></span> <span data-ttu-id="eec28-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="eec28-184">uploadState</span></span>|<span data-ttu-id="eec28-185">Int32</span><span class="sxs-lookup"><span data-stu-id="eec28-185">Int32</span></span>|<span data-ttu-id="eec28-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="eec28-186">The upload state.</span></span> <span data-ttu-id="eec28-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="eec28-188">publishingState</span></span>|[<span data-ttu-id="eec28-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="eec28-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="eec28-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eec28-190">The publishing state for the app.</span></span> <span data-ttu-id="eec28-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="eec28-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eec28-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eec28-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="eec28-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="eec28-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="eec28-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="eec28-194">isAssigned</span></span>|<span data-ttu-id="eec28-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="eec28-195">Boolean</span></span>|<span data-ttu-id="eec28-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="eec28-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="eec28-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eec28-198">roleScopeTagIds</span></span>|<span data-ttu-id="eec28-199">String collection</span><span class="sxs-lookup"><span data-stu-id="eec28-199">String collection</span></span>|<span data-ttu-id="eec28-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="eec28-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="eec28-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="eec28-202">dependentAppCount</span></span>|<span data-ttu-id="eec28-203">Int32</span><span class="sxs-lookup"><span data-stu-id="eec28-203">Int32</span></span>|<span data-ttu-id="eec28-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="eec28-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="eec28-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eec28-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="eec28-206">packageId</span><span class="sxs-lookup"><span data-stu-id="eec28-206">packageId</span></span>|<span data-ttu-id="eec28-207">String</span><span class="sxs-lookup"><span data-stu-id="eec28-207">String</span></span>|<span data-ttu-id="eec28-208">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="eec28-208">The package identifier.</span></span>|
|<span data-ttu-id="eec28-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="eec28-209">appIdentifier</span></span>|<span data-ttu-id="eec28-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eec28-210">String</span></span>|<span data-ttu-id="eec28-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="eec28-211">The Identity Name.</span></span>|
|<span data-ttu-id="eec28-212">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="eec28-212">usedLicenseCount</span></span>|<span data-ttu-id="eec28-213">Int32</span><span class="sxs-lookup"><span data-stu-id="eec28-213">Int32</span></span>|<span data-ttu-id="eec28-214">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="eec28-214">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="eec28-215">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="eec28-215">totalLicenseCount</span></span>|<span data-ttu-id="eec28-216">Int32</span><span class="sxs-lookup"><span data-stu-id="eec28-216">Int32</span></span>|<span data-ttu-id="eec28-217">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="eec28-217">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="eec28-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="eec28-218">appStoreUrl</span></span>|<span data-ttu-id="eec28-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eec28-219">String</span></span>|<span data-ttu-id="eec28-220">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="eec28-220">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="eec28-221">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="eec28-221">isPrivate</span></span>|<span data-ttu-id="eec28-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="eec28-222">Boolean</span></span>|<span data-ttu-id="eec28-223">Indica se o aplicativo está disponível somente para os usuários de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="eec28-223">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="eec28-224">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="eec28-224">isSystemApp</span></span>|<span data-ttu-id="eec28-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="eec28-225">Boolean</span></span>|<span data-ttu-id="eec28-226">Indica se o aplicativo é um aplicativo de sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="eec28-226">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="eec28-227">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="eec28-227">supportsOemConfig</span></span>|<span data-ttu-id="eec28-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="eec28-228">Boolean</span></span>|<span data-ttu-id="eec28-229">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="eec28-229">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="eec28-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="eec28-230">Response</span></span>
<span data-ttu-id="eec28-231">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eec28-231">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eec28-232">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eec28-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="eec28-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eec28-233">Request</span></span>
<span data-ttu-id="eec28-234">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eec28-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 984

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
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="eec28-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="eec28-235">Response</span></span>
<span data-ttu-id="eec28-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eec28-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1156

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
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```





