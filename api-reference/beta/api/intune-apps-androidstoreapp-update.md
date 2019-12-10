---
title: Atualizar androidStoreApp
description: Atualiza as propriedades de um objeto androidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff85a8e7ced96788a9d64b0014099a77d437b9a3
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39921813"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="a59b0-103">Atualizar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="a59b0-103">Update androidStoreApp</span></span>

> <span data-ttu-id="a59b0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a59b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a59b0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a59b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a59b0-106">Atualiza as propriedades de um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="a59b0-106">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a59b0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a59b0-107">Prerequisites</span></span>
<span data-ttu-id="a59b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a59b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a59b0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a59b0-110">Permission type</span></span>|<span data-ttu-id="a59b0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a59b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a59b0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a59b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a59b0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a59b0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a59b0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a59b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a59b0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a59b0-115">Not supported.</span></span>|
|<span data-ttu-id="a59b0-116">Application</span><span class="sxs-lookup"><span data-stu-id="a59b0-116">Application</span></span>|<span data-ttu-id="a59b0-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a59b0-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a59b0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a59b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a59b0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a59b0-119">Request headers</span></span>
|<span data-ttu-id="a59b0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a59b0-120">Header</span></span>|<span data-ttu-id="a59b0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a59b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a59b0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a59b0-122">Authorization</span></span>|<span data-ttu-id="a59b0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a59b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a59b0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a59b0-124">Accept</span></span>|<span data-ttu-id="a59b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a59b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a59b0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a59b0-126">Request body</span></span>
<span data-ttu-id="a59b0-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="a59b0-127">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="a59b0-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="a59b0-128">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="a59b0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a59b0-129">Property</span></span>|<span data-ttu-id="a59b0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a59b0-130">Type</span></span>|<span data-ttu-id="a59b0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a59b0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a59b0-132">id</span><span class="sxs-lookup"><span data-stu-id="a59b0-132">id</span></span>|<span data-ttu-id="a59b0-133">String</span><span class="sxs-lookup"><span data-stu-id="a59b0-133">String</span></span>|<span data-ttu-id="a59b0-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a59b0-134">Key of the entity.</span></span> <span data-ttu-id="a59b0-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a59b0-136">displayName</span></span>|<span data-ttu-id="a59b0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59b0-137">String</span></span>|<span data-ttu-id="a59b0-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a59b0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a59b0-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-140">description</span><span class="sxs-lookup"><span data-stu-id="a59b0-140">description</span></span>|<span data-ttu-id="a59b0-141">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a59b0-141">String</span></span>|<span data-ttu-id="a59b0-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a59b0-142">The description of the app.</span></span> <span data-ttu-id="a59b0-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-144">publicador</span><span class="sxs-lookup"><span data-stu-id="a59b0-144">publisher</span></span>|<span data-ttu-id="a59b0-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a59b0-145">String</span></span>|<span data-ttu-id="a59b0-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a59b0-146">The publisher of the app.</span></span> <span data-ttu-id="a59b0-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a59b0-148">largeIcon</span></span>|[<span data-ttu-id="a59b0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a59b0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a59b0-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="a59b0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a59b0-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a59b0-152">createdDateTime</span></span>|<span data-ttu-id="a59b0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a59b0-153">DateTimeOffset</span></span>|<span data-ttu-id="a59b0-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a59b0-154">The date and time the app was created.</span></span> <span data-ttu-id="a59b0-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a59b0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a59b0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a59b0-157">DateTimeOffset</span></span>|<span data-ttu-id="a59b0-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a59b0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a59b0-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a59b0-160">isFeatured</span></span>|<span data-ttu-id="a59b0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a59b0-161">Boolean</span></span>|<span data-ttu-id="a59b0-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a59b0-163">privacyInformationUrl</span></span>|<span data-ttu-id="a59b0-164">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a59b0-164">String</span></span>|<span data-ttu-id="a59b0-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="a59b0-165">The privacy statement Url.</span></span> <span data-ttu-id="a59b0-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a59b0-167">informationUrl</span></span>|<span data-ttu-id="a59b0-168">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a59b0-168">String</span></span>|<span data-ttu-id="a59b0-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="a59b0-169">The more information Url.</span></span> <span data-ttu-id="a59b0-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-171">owner</span><span class="sxs-lookup"><span data-stu-id="a59b0-171">owner</span></span>|<span data-ttu-id="a59b0-172">String</span><span class="sxs-lookup"><span data-stu-id="a59b0-172">String</span></span>|<span data-ttu-id="a59b0-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a59b0-173">The owner of the app.</span></span> <span data-ttu-id="a59b0-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-175">developer</span><span class="sxs-lookup"><span data-stu-id="a59b0-175">developer</span></span>|<span data-ttu-id="a59b0-176">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a59b0-176">String</span></span>|<span data-ttu-id="a59b0-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a59b0-177">The developer of the app.</span></span> <span data-ttu-id="a59b0-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-179">notes</span><span class="sxs-lookup"><span data-stu-id="a59b0-179">notes</span></span>|<span data-ttu-id="a59b0-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a59b0-180">String</span></span>|<span data-ttu-id="a59b0-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a59b0-181">Notes for the app.</span></span> <span data-ttu-id="a59b0-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a59b0-183">uploadState</span></span>|<span data-ttu-id="a59b0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a59b0-184">Int32</span></span>|<span data-ttu-id="a59b0-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="a59b0-185">The upload state.</span></span> <span data-ttu-id="a59b0-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a59b0-187">publishingState</span></span>|[<span data-ttu-id="a59b0-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a59b0-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a59b0-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a59b0-189">The publishing state for the app.</span></span> <span data-ttu-id="a59b0-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="a59b0-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a59b0-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a59b0-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="a59b0-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a59b0-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a59b0-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a59b0-193">isAssigned</span></span>|<span data-ttu-id="a59b0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a59b0-194">Boolean</span></span>|<span data-ttu-id="a59b0-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="a59b0-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a59b0-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a59b0-197">roleScopeTagIds</span></span>|<span data-ttu-id="a59b0-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59b0-198">String collection</span></span>|<span data-ttu-id="a59b0-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="a59b0-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a59b0-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="a59b0-201">dependentAppCount</span></span>|<span data-ttu-id="a59b0-202">Int32</span><span class="sxs-lookup"><span data-stu-id="a59b0-202">Int32</span></span>|<span data-ttu-id="a59b0-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="a59b0-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a59b0-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59b0-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a59b0-205">packageId</span><span class="sxs-lookup"><span data-stu-id="a59b0-205">packageId</span></span>|<span data-ttu-id="a59b0-206">String</span><span class="sxs-lookup"><span data-stu-id="a59b0-206">String</span></span>|<span data-ttu-id="a59b0-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="a59b0-207">The package identifier.</span></span>|
|<span data-ttu-id="a59b0-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="a59b0-208">appIdentifier</span></span>|<span data-ttu-id="a59b0-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59b0-209">String</span></span>|<span data-ttu-id="a59b0-210">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="a59b0-210">The Identity Name.</span></span>|
|<span data-ttu-id="a59b0-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a59b0-211">appStoreUrl</span></span>|<span data-ttu-id="a59b0-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59b0-212">String</span></span>|<span data-ttu-id="a59b0-213">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="a59b0-213">The Android app store URL.</span></span>|
|<span data-ttu-id="a59b0-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a59b0-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a59b0-215">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a59b0-215">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="a59b0-216">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="a59b0-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="a59b0-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="a59b0-217">Response</span></span>
<span data-ttu-id="a59b0-218">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a59b0-218">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a59b0-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a59b0-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="a59b0-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a59b0-220">Request</span></span>
<span data-ttu-id="a59b0-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a59b0-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1230

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="a59b0-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="a59b0-222">Response</span></span>
<span data-ttu-id="a59b0-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a59b0-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1402

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```





