---
title: Atualizar androidForWorkApp
description: Atualiza as propriedades de um objeto androidForWorkApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 858210d808d42efa11db42834f655a48ba6f1f0d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37178155"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="87721-103">Atualizar androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="87721-103">Update androidForWorkApp</span></span>

> <span data-ttu-id="87721-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87721-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87721-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87721-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87721-106">Atualiza as propriedades de um objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="87721-106">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87721-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87721-107">Prerequisites</span></span>
<span data-ttu-id="87721-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87721-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87721-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87721-110">Permission type</span></span>|<span data-ttu-id="87721-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87721-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87721-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87721-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87721-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87721-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="87721-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87721-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87721-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87721-115">Not supported.</span></span>|
|<span data-ttu-id="87721-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87721-116">Application</span></span>|<span data-ttu-id="87721-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87721-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87721-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87721-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="87721-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87721-119">Request headers</span></span>
|<span data-ttu-id="87721-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87721-120">Header</span></span>|<span data-ttu-id="87721-121">Valor</span><span class="sxs-lookup"><span data-stu-id="87721-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87721-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="87721-122">Authorization</span></span>|<span data-ttu-id="87721-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87721-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87721-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87721-124">Accept</span></span>|<span data-ttu-id="87721-125">application/json</span><span class="sxs-lookup"><span data-stu-id="87721-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87721-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87721-126">Request body</span></span>
<span data-ttu-id="87721-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="87721-127">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="87721-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span><span class="sxs-lookup"><span data-stu-id="87721-128">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="87721-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87721-129">Property</span></span>|<span data-ttu-id="87721-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="87721-130">Type</span></span>|<span data-ttu-id="87721-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="87721-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87721-132">id</span><span class="sxs-lookup"><span data-stu-id="87721-132">id</span></span>|<span data-ttu-id="87721-133">String</span><span class="sxs-lookup"><span data-stu-id="87721-133">String</span></span>|<span data-ttu-id="87721-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="87721-134">Key of the entity.</span></span> <span data-ttu-id="87721-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-136">displayName</span><span class="sxs-lookup"><span data-stu-id="87721-136">displayName</span></span>|<span data-ttu-id="87721-137">String</span><span class="sxs-lookup"><span data-stu-id="87721-137">String</span></span>|<span data-ttu-id="87721-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="87721-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="87721-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-140">descrição</span><span class="sxs-lookup"><span data-stu-id="87721-140">description</span></span>|<span data-ttu-id="87721-141">String</span><span class="sxs-lookup"><span data-stu-id="87721-141">String</span></span>|<span data-ttu-id="87721-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="87721-142">The description of the app.</span></span> <span data-ttu-id="87721-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-144">publicador</span><span class="sxs-lookup"><span data-stu-id="87721-144">publisher</span></span>|<span data-ttu-id="87721-145">String</span><span class="sxs-lookup"><span data-stu-id="87721-145">String</span></span>|<span data-ttu-id="87721-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="87721-146">The publisher of the app.</span></span> <span data-ttu-id="87721-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="87721-148">largeIcon</span></span>|[<span data-ttu-id="87721-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="87721-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="87721-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="87721-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="87721-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87721-152">createdDateTime</span></span>|<span data-ttu-id="87721-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87721-153">DateTimeOffset</span></span>|<span data-ttu-id="87721-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="87721-154">The date and time the app was created.</span></span> <span data-ttu-id="87721-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87721-156">lastModifiedDateTime</span></span>|<span data-ttu-id="87721-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87721-157">DateTimeOffset</span></span>|<span data-ttu-id="87721-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="87721-158">The date and time the app was last modified.</span></span> <span data-ttu-id="87721-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="87721-160">isFeatured</span></span>|<span data-ttu-id="87721-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="87721-161">Boolean</span></span>|<span data-ttu-id="87721-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="87721-163">privacyInformationUrl</span></span>|<span data-ttu-id="87721-164">String</span><span class="sxs-lookup"><span data-stu-id="87721-164">String</span></span>|<span data-ttu-id="87721-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="87721-165">The privacy statement Url.</span></span> <span data-ttu-id="87721-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="87721-167">informationUrl</span></span>|<span data-ttu-id="87721-168">String</span><span class="sxs-lookup"><span data-stu-id="87721-168">String</span></span>|<span data-ttu-id="87721-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="87721-169">The more information Url.</span></span> <span data-ttu-id="87721-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-171">owner</span><span class="sxs-lookup"><span data-stu-id="87721-171">owner</span></span>|<span data-ttu-id="87721-172">String</span><span class="sxs-lookup"><span data-stu-id="87721-172">String</span></span>|<span data-ttu-id="87721-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="87721-173">The owner of the app.</span></span> <span data-ttu-id="87721-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-175">developer</span><span class="sxs-lookup"><span data-stu-id="87721-175">developer</span></span>|<span data-ttu-id="87721-176">String</span><span class="sxs-lookup"><span data-stu-id="87721-176">String</span></span>|<span data-ttu-id="87721-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="87721-177">The developer of the app.</span></span> <span data-ttu-id="87721-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-179">notes</span><span class="sxs-lookup"><span data-stu-id="87721-179">notes</span></span>|<span data-ttu-id="87721-180">String</span><span class="sxs-lookup"><span data-stu-id="87721-180">String</span></span>|<span data-ttu-id="87721-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="87721-181">Notes for the app.</span></span> <span data-ttu-id="87721-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="87721-183">uploadState</span></span>|<span data-ttu-id="87721-184">Int32</span><span class="sxs-lookup"><span data-stu-id="87721-184">Int32</span></span>|<span data-ttu-id="87721-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="87721-185">The upload state.</span></span> <span data-ttu-id="87721-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="87721-187">publishingState</span></span>|[<span data-ttu-id="87721-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="87721-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="87721-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="87721-189">The publishing state for the app.</span></span> <span data-ttu-id="87721-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="87721-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="87721-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87721-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="87721-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="87721-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="87721-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="87721-193">isAssigned</span></span>|<span data-ttu-id="87721-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="87721-194">Boolean</span></span>|<span data-ttu-id="87721-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="87721-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="87721-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="87721-197">roleScopeTagIds</span></span>|<span data-ttu-id="87721-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="87721-198">String collection</span></span>|<span data-ttu-id="87721-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="87721-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="87721-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="87721-201">dependentAppCount</span></span>|<span data-ttu-id="87721-202">Int32</span><span class="sxs-lookup"><span data-stu-id="87721-202">Int32</span></span>|<span data-ttu-id="87721-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="87721-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="87721-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87721-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87721-205">packageId</span><span class="sxs-lookup"><span data-stu-id="87721-205">packageId</span></span>|<span data-ttu-id="87721-206">String</span><span class="sxs-lookup"><span data-stu-id="87721-206">String</span></span>|<span data-ttu-id="87721-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="87721-207">The package identifier.</span></span>|
|<span data-ttu-id="87721-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="87721-208">appIdentifier</span></span>|<span data-ttu-id="87721-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87721-209">String</span></span>|<span data-ttu-id="87721-210">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="87721-210">The Identity Name.</span></span>|
|<span data-ttu-id="87721-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="87721-211">usedLicenseCount</span></span>|<span data-ttu-id="87721-212">Int32</span><span class="sxs-lookup"><span data-stu-id="87721-212">Int32</span></span>|<span data-ttu-id="87721-213">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="87721-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="87721-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="87721-214">totalLicenseCount</span></span>|<span data-ttu-id="87721-215">Int32</span><span class="sxs-lookup"><span data-stu-id="87721-215">Int32</span></span>|<span data-ttu-id="87721-216">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="87721-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="87721-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="87721-217">appStoreUrl</span></span>|<span data-ttu-id="87721-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87721-218">String</span></span>|<span data-ttu-id="87721-219">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="87721-219">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="87721-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="87721-220">Response</span></span>
<span data-ttu-id="87721-221">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87721-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87721-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87721-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="87721-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87721-223">Request</span></span>
<span data-ttu-id="87721-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87721-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="87721-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="87721-225">Response</span></span>
<span data-ttu-id="87721-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87721-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




