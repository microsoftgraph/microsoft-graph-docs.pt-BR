---
title: Atualizar androidForWorkApp
description: Atualiza as propriedades de um objeto androidForWorkApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 90b162629711ff6fa120552dde36dc0447f93321
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417761"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="afb23-103">Atualizar androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="afb23-103">Update androidForWorkApp</span></span>

<span data-ttu-id="afb23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afb23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afb23-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="afb23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afb23-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="afb23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afb23-107">Atualiza as propriedades de um objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="afb23-107">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afb23-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="afb23-108">Prerequisites</span></span>
<span data-ttu-id="afb23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afb23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afb23-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afb23-111">Permission type</span></span>|<span data-ttu-id="afb23-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="afb23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afb23-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afb23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afb23-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb23-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="afb23-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afb23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afb23-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afb23-116">Not supported.</span></span>|
|<span data-ttu-id="afb23-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afb23-117">Application</span></span>|<span data-ttu-id="afb23-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb23-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afb23-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afb23-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="afb23-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afb23-120">Request headers</span></span>
|<span data-ttu-id="afb23-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="afb23-121">Header</span></span>|<span data-ttu-id="afb23-122">Valor</span><span class="sxs-lookup"><span data-stu-id="afb23-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afb23-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="afb23-123">Authorization</span></span>|<span data-ttu-id="afb23-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afb23-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afb23-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="afb23-125">Accept</span></span>|<span data-ttu-id="afb23-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afb23-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afb23-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afb23-127">Request body</span></span>
<span data-ttu-id="afb23-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="afb23-128">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="afb23-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span><span class="sxs-lookup"><span data-stu-id="afb23-129">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="afb23-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afb23-130">Property</span></span>|<span data-ttu-id="afb23-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="afb23-131">Type</span></span>|<span data-ttu-id="afb23-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="afb23-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afb23-133">id</span><span class="sxs-lookup"><span data-stu-id="afb23-133">id</span></span>|<span data-ttu-id="afb23-134">String</span><span class="sxs-lookup"><span data-stu-id="afb23-134">String</span></span>|<span data-ttu-id="afb23-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="afb23-135">Key of the entity.</span></span> <span data-ttu-id="afb23-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-137">displayName</span><span class="sxs-lookup"><span data-stu-id="afb23-137">displayName</span></span>|<span data-ttu-id="afb23-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afb23-138">String</span></span>|<span data-ttu-id="afb23-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="afb23-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="afb23-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-141">description</span><span class="sxs-lookup"><span data-stu-id="afb23-141">description</span></span>|<span data-ttu-id="afb23-142">String</span><span class="sxs-lookup"><span data-stu-id="afb23-142">String</span></span>|<span data-ttu-id="afb23-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="afb23-143">The description of the app.</span></span> <span data-ttu-id="afb23-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-145">publicador</span><span class="sxs-lookup"><span data-stu-id="afb23-145">publisher</span></span>|<span data-ttu-id="afb23-146">String</span><span class="sxs-lookup"><span data-stu-id="afb23-146">String</span></span>|<span data-ttu-id="afb23-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="afb23-147">The publisher of the app.</span></span> <span data-ttu-id="afb23-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="afb23-149">largeIcon</span></span>|[<span data-ttu-id="afb23-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="afb23-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="afb23-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="afb23-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="afb23-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="afb23-153">createdDateTime</span></span>|<span data-ttu-id="afb23-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afb23-154">DateTimeOffset</span></span>|<span data-ttu-id="afb23-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="afb23-155">The date and time the app was created.</span></span> <span data-ttu-id="afb23-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="afb23-157">lastModifiedDateTime</span></span>|<span data-ttu-id="afb23-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afb23-158">DateTimeOffset</span></span>|<span data-ttu-id="afb23-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="afb23-159">The date and time the app was last modified.</span></span> <span data-ttu-id="afb23-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="afb23-161">isFeatured</span></span>|<span data-ttu-id="afb23-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="afb23-162">Boolean</span></span>|<span data-ttu-id="afb23-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="afb23-164">privacyInformationUrl</span></span>|<span data-ttu-id="afb23-165">String</span><span class="sxs-lookup"><span data-stu-id="afb23-165">String</span></span>|<span data-ttu-id="afb23-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="afb23-166">The privacy statement Url.</span></span> <span data-ttu-id="afb23-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="afb23-168">informationUrl</span></span>|<span data-ttu-id="afb23-169">String</span><span class="sxs-lookup"><span data-stu-id="afb23-169">String</span></span>|<span data-ttu-id="afb23-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="afb23-170">The more information Url.</span></span> <span data-ttu-id="afb23-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-172">owner</span><span class="sxs-lookup"><span data-stu-id="afb23-172">owner</span></span>|<span data-ttu-id="afb23-173">String</span><span class="sxs-lookup"><span data-stu-id="afb23-173">String</span></span>|<span data-ttu-id="afb23-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="afb23-174">The owner of the app.</span></span> <span data-ttu-id="afb23-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-176">developer</span><span class="sxs-lookup"><span data-stu-id="afb23-176">developer</span></span>|<span data-ttu-id="afb23-177">String</span><span class="sxs-lookup"><span data-stu-id="afb23-177">String</span></span>|<span data-ttu-id="afb23-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="afb23-178">The developer of the app.</span></span> <span data-ttu-id="afb23-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-180">notes</span><span class="sxs-lookup"><span data-stu-id="afb23-180">notes</span></span>|<span data-ttu-id="afb23-181">String</span><span class="sxs-lookup"><span data-stu-id="afb23-181">String</span></span>|<span data-ttu-id="afb23-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="afb23-182">Notes for the app.</span></span> <span data-ttu-id="afb23-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="afb23-184">uploadState</span></span>|<span data-ttu-id="afb23-185">Int32</span><span class="sxs-lookup"><span data-stu-id="afb23-185">Int32</span></span>|<span data-ttu-id="afb23-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="afb23-186">The upload state.</span></span> <span data-ttu-id="afb23-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="afb23-188">publishingState</span></span>|[<span data-ttu-id="afb23-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="afb23-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="afb23-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="afb23-190">The publishing state for the app.</span></span> <span data-ttu-id="afb23-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="afb23-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="afb23-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="afb23-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="afb23-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="afb23-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="afb23-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="afb23-194">isAssigned</span></span>|<span data-ttu-id="afb23-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="afb23-195">Boolean</span></span>|<span data-ttu-id="afb23-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="afb23-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="afb23-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="afb23-198">roleScopeTagIds</span></span>|<span data-ttu-id="afb23-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="afb23-199">String collection</span></span>|<span data-ttu-id="afb23-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="afb23-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="afb23-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="afb23-202">dependentAppCount</span></span>|<span data-ttu-id="afb23-203">Int32</span><span class="sxs-lookup"><span data-stu-id="afb23-203">Int32</span></span>|<span data-ttu-id="afb23-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="afb23-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="afb23-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afb23-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="afb23-206">packageId</span><span class="sxs-lookup"><span data-stu-id="afb23-206">packageId</span></span>|<span data-ttu-id="afb23-207">String</span><span class="sxs-lookup"><span data-stu-id="afb23-207">String</span></span>|<span data-ttu-id="afb23-208">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="afb23-208">The package identifier.</span></span>|
|<span data-ttu-id="afb23-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="afb23-209">appIdentifier</span></span>|<span data-ttu-id="afb23-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afb23-210">String</span></span>|<span data-ttu-id="afb23-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="afb23-211">The Identity Name.</span></span>|
|<span data-ttu-id="afb23-212">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="afb23-212">usedLicenseCount</span></span>|<span data-ttu-id="afb23-213">Int32</span><span class="sxs-lookup"><span data-stu-id="afb23-213">Int32</span></span>|<span data-ttu-id="afb23-214">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="afb23-214">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="afb23-215">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="afb23-215">totalLicenseCount</span></span>|<span data-ttu-id="afb23-216">Int32</span><span class="sxs-lookup"><span data-stu-id="afb23-216">Int32</span></span>|<span data-ttu-id="afb23-217">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="afb23-217">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="afb23-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="afb23-218">appStoreUrl</span></span>|<span data-ttu-id="afb23-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afb23-219">String</span></span>|<span data-ttu-id="afb23-220">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="afb23-220">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="afb23-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="afb23-221">Response</span></span>
<span data-ttu-id="afb23-222">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afb23-222">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afb23-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afb23-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="afb23-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afb23-224">Request</span></span>
<span data-ttu-id="afb23-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="afb23-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 903

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="afb23-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="afb23-226">Response</span></span>
<span data-ttu-id="afb23-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afb23-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1075

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```



