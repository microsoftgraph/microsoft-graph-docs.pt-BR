---
title: Atualizar androidForWorkApp
description: Atualiza as propriedades de um objeto androidForWorkApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43aee40395ab9ca4c9f5b4f575e0611e432fc029
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762368"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="ed459-103">Atualizar androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="ed459-103">Update androidForWorkApp</span></span>

> <span data-ttu-id="ed459-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed459-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed459-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed459-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed459-106">Atualiza as propriedades de um objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ed459-106">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed459-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed459-107">Prerequisites</span></span>
<span data-ttu-id="ed459-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed459-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed459-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed459-110">Permission type</span></span>|<span data-ttu-id="ed459-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed459-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed459-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed459-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed459-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed459-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ed459-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed459-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed459-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed459-115">Not supported.</span></span>|
|<span data-ttu-id="ed459-116">Application</span><span class="sxs-lookup"><span data-stu-id="ed459-116">Application</span></span>|<span data-ttu-id="ed459-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed459-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed459-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed459-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ed459-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed459-119">Request headers</span></span>
|<span data-ttu-id="ed459-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed459-120">Header</span></span>|<span data-ttu-id="ed459-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ed459-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed459-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed459-122">Authorization</span></span>|<span data-ttu-id="ed459-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed459-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed459-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed459-124">Accept</span></span>|<span data-ttu-id="ed459-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed459-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed459-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed459-126">Request body</span></span>
<span data-ttu-id="ed459-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ed459-127">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="ed459-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span><span class="sxs-lookup"><span data-stu-id="ed459-128">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="ed459-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed459-129">Property</span></span>|<span data-ttu-id="ed459-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed459-130">Type</span></span>|<span data-ttu-id="ed459-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed459-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed459-132">id</span><span class="sxs-lookup"><span data-stu-id="ed459-132">id</span></span>|<span data-ttu-id="ed459-133">String</span><span class="sxs-lookup"><span data-stu-id="ed459-133">String</span></span>|<span data-ttu-id="ed459-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ed459-134">Key of the entity.</span></span> <span data-ttu-id="ed459-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ed459-136">displayName</span></span>|<span data-ttu-id="ed459-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed459-137">String</span></span>|<span data-ttu-id="ed459-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ed459-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ed459-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-140">description</span><span class="sxs-lookup"><span data-stu-id="ed459-140">description</span></span>|<span data-ttu-id="ed459-141">String</span><span class="sxs-lookup"><span data-stu-id="ed459-141">String</span></span>|<span data-ttu-id="ed459-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed459-142">The description of the app.</span></span> <span data-ttu-id="ed459-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-144">publicador</span><span class="sxs-lookup"><span data-stu-id="ed459-144">publisher</span></span>|<span data-ttu-id="ed459-145">String</span><span class="sxs-lookup"><span data-stu-id="ed459-145">String</span></span>|<span data-ttu-id="ed459-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed459-146">The publisher of the app.</span></span> <span data-ttu-id="ed459-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ed459-148">largeIcon</span></span>|[<span data-ttu-id="ed459-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ed459-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ed459-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ed459-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ed459-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed459-152">createdDateTime</span></span>|<span data-ttu-id="ed459-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed459-153">DateTimeOffset</span></span>|<span data-ttu-id="ed459-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed459-154">The date and time the app was created.</span></span> <span data-ttu-id="ed459-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed459-156">lastModifiedDateTime</span></span>|<span data-ttu-id="ed459-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed459-157">DateTimeOffset</span></span>|<span data-ttu-id="ed459-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ed459-158">The date and time the app was last modified.</span></span> <span data-ttu-id="ed459-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ed459-160">isFeatured</span></span>|<span data-ttu-id="ed459-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed459-161">Boolean</span></span>|<span data-ttu-id="ed459-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ed459-163">privacyInformationUrl</span></span>|<span data-ttu-id="ed459-164">String</span><span class="sxs-lookup"><span data-stu-id="ed459-164">String</span></span>|<span data-ttu-id="ed459-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ed459-165">The privacy statement Url.</span></span> <span data-ttu-id="ed459-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ed459-167">informationUrl</span></span>|<span data-ttu-id="ed459-168">String</span><span class="sxs-lookup"><span data-stu-id="ed459-168">String</span></span>|<span data-ttu-id="ed459-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ed459-169">The more information Url.</span></span> <span data-ttu-id="ed459-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-171">owner</span><span class="sxs-lookup"><span data-stu-id="ed459-171">owner</span></span>|<span data-ttu-id="ed459-172">String</span><span class="sxs-lookup"><span data-stu-id="ed459-172">String</span></span>|<span data-ttu-id="ed459-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ed459-173">The owner of the app.</span></span> <span data-ttu-id="ed459-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-175">developer</span><span class="sxs-lookup"><span data-stu-id="ed459-175">developer</span></span>|<span data-ttu-id="ed459-176">String</span><span class="sxs-lookup"><span data-stu-id="ed459-176">String</span></span>|<span data-ttu-id="ed459-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed459-177">The developer of the app.</span></span> <span data-ttu-id="ed459-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-179">notes</span><span class="sxs-lookup"><span data-stu-id="ed459-179">notes</span></span>|<span data-ttu-id="ed459-180">String</span><span class="sxs-lookup"><span data-stu-id="ed459-180">String</span></span>|<span data-ttu-id="ed459-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed459-181">Notes for the app.</span></span> <span data-ttu-id="ed459-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="ed459-183">uploadState</span></span>|<span data-ttu-id="ed459-184">Int32</span><span class="sxs-lookup"><span data-stu-id="ed459-184">Int32</span></span>|<span data-ttu-id="ed459-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="ed459-185">The upload state.</span></span> <span data-ttu-id="ed459-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="ed459-187">publishingState</span></span>|[<span data-ttu-id="ed459-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ed459-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ed459-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed459-189">The publishing state for the app.</span></span> <span data-ttu-id="ed459-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ed459-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ed459-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ed459-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ed459-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ed459-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ed459-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ed459-193">isAssigned</span></span>|<span data-ttu-id="ed459-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed459-194">Boolean</span></span>|<span data-ttu-id="ed459-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="ed459-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ed459-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ed459-197">roleScopeTagIds</span></span>|<span data-ttu-id="ed459-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed459-198">String collection</span></span>|<span data-ttu-id="ed459-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ed459-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ed459-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ed459-201">dependentAppCount</span></span>|<span data-ttu-id="ed459-202">Int32</span><span class="sxs-lookup"><span data-stu-id="ed459-202">Int32</span></span>|<span data-ttu-id="ed459-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="ed459-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ed459-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed459-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ed459-205">packageId</span><span class="sxs-lookup"><span data-stu-id="ed459-205">packageId</span></span>|<span data-ttu-id="ed459-206">String</span><span class="sxs-lookup"><span data-stu-id="ed459-206">String</span></span>|<span data-ttu-id="ed459-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="ed459-207">The package identifier.</span></span>|
|<span data-ttu-id="ed459-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="ed459-208">appIdentifier</span></span>|<span data-ttu-id="ed459-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed459-209">String</span></span>|<span data-ttu-id="ed459-210">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ed459-210">The Identity Name.</span></span>|
|<span data-ttu-id="ed459-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ed459-211">usedLicenseCount</span></span>|<span data-ttu-id="ed459-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ed459-212">Int32</span></span>|<span data-ttu-id="ed459-213">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="ed459-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="ed459-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ed459-214">totalLicenseCount</span></span>|<span data-ttu-id="ed459-215">Int32</span><span class="sxs-lookup"><span data-stu-id="ed459-215">Int32</span></span>|<span data-ttu-id="ed459-216">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="ed459-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="ed459-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ed459-217">appStoreUrl</span></span>|<span data-ttu-id="ed459-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed459-218">String</span></span>|<span data-ttu-id="ed459-219">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="ed459-219">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="ed459-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed459-220">Response</span></span>
<span data-ttu-id="ed459-221">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed459-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed459-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed459-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed459-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed459-223">Request</span></span>
<span data-ttu-id="ed459-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed459-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ed459-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed459-225">Response</span></span>
<span data-ttu-id="ed459-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed459-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




