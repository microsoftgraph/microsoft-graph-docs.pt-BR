---
title: Criar androidForWorkApp
description: Criar um novo objeto androidForWorkApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1db34a26ffcf503ce69de10de832733bc47b02f7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762396"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="34bef-103">Criar androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="34bef-103">Create androidForWorkApp</span></span>

> <span data-ttu-id="34bef-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34bef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34bef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34bef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34bef-106">Criar um novo objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="34bef-106">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34bef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34bef-107">Prerequisites</span></span>
<span data-ttu-id="34bef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34bef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34bef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34bef-110">Permission type</span></span>|<span data-ttu-id="34bef-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34bef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34bef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34bef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34bef-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34bef-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="34bef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34bef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34bef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34bef-115">Not supported.</span></span>|
|<span data-ttu-id="34bef-116">Application</span><span class="sxs-lookup"><span data-stu-id="34bef-116">Application</span></span>|<span data-ttu-id="34bef-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34bef-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34bef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34bef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="34bef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34bef-119">Request headers</span></span>
|<span data-ttu-id="34bef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34bef-120">Header</span></span>|<span data-ttu-id="34bef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="34bef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34bef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34bef-122">Authorization</span></span>|<span data-ttu-id="34bef-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34bef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34bef-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34bef-124">Accept</span></span>|<span data-ttu-id="34bef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34bef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34bef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34bef-126">Request body</span></span>
<span data-ttu-id="34bef-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkApp.</span><span class="sxs-lookup"><span data-stu-id="34bef-127">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="34bef-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkApp.</span><span class="sxs-lookup"><span data-stu-id="34bef-128">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="34bef-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34bef-129">Property</span></span>|<span data-ttu-id="34bef-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="34bef-130">Type</span></span>|<span data-ttu-id="34bef-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="34bef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34bef-132">id</span><span class="sxs-lookup"><span data-stu-id="34bef-132">id</span></span>|<span data-ttu-id="34bef-133">String</span><span class="sxs-lookup"><span data-stu-id="34bef-133">String</span></span>|<span data-ttu-id="34bef-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="34bef-134">Key of the entity.</span></span> <span data-ttu-id="34bef-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-136">displayName</span><span class="sxs-lookup"><span data-stu-id="34bef-136">displayName</span></span>|<span data-ttu-id="34bef-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34bef-137">String</span></span>|<span data-ttu-id="34bef-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="34bef-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="34bef-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-140">description</span><span class="sxs-lookup"><span data-stu-id="34bef-140">description</span></span>|<span data-ttu-id="34bef-141">String</span><span class="sxs-lookup"><span data-stu-id="34bef-141">String</span></span>|<span data-ttu-id="34bef-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34bef-142">The description of the app.</span></span> <span data-ttu-id="34bef-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-144">publicador</span><span class="sxs-lookup"><span data-stu-id="34bef-144">publisher</span></span>|<span data-ttu-id="34bef-145">String</span><span class="sxs-lookup"><span data-stu-id="34bef-145">String</span></span>|<span data-ttu-id="34bef-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34bef-146">The publisher of the app.</span></span> <span data-ttu-id="34bef-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="34bef-148">largeIcon</span></span>|[<span data-ttu-id="34bef-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="34bef-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="34bef-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="34bef-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="34bef-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34bef-152">createdDateTime</span></span>|<span data-ttu-id="34bef-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34bef-153">DateTimeOffset</span></span>|<span data-ttu-id="34bef-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34bef-154">The date and time the app was created.</span></span> <span data-ttu-id="34bef-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34bef-156">lastModifiedDateTime</span></span>|<span data-ttu-id="34bef-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34bef-157">DateTimeOffset</span></span>|<span data-ttu-id="34bef-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="34bef-158">The date and time the app was last modified.</span></span> <span data-ttu-id="34bef-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="34bef-160">isFeatured</span></span>|<span data-ttu-id="34bef-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="34bef-161">Boolean</span></span>|<span data-ttu-id="34bef-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="34bef-163">privacyInformationUrl</span></span>|<span data-ttu-id="34bef-164">String</span><span class="sxs-lookup"><span data-stu-id="34bef-164">String</span></span>|<span data-ttu-id="34bef-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="34bef-165">The privacy statement Url.</span></span> <span data-ttu-id="34bef-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="34bef-167">informationUrl</span></span>|<span data-ttu-id="34bef-168">String</span><span class="sxs-lookup"><span data-stu-id="34bef-168">String</span></span>|<span data-ttu-id="34bef-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="34bef-169">The more information Url.</span></span> <span data-ttu-id="34bef-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-171">owner</span><span class="sxs-lookup"><span data-stu-id="34bef-171">owner</span></span>|<span data-ttu-id="34bef-172">String</span><span class="sxs-lookup"><span data-stu-id="34bef-172">String</span></span>|<span data-ttu-id="34bef-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="34bef-173">The owner of the app.</span></span> <span data-ttu-id="34bef-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-175">developer</span><span class="sxs-lookup"><span data-stu-id="34bef-175">developer</span></span>|<span data-ttu-id="34bef-176">String</span><span class="sxs-lookup"><span data-stu-id="34bef-176">String</span></span>|<span data-ttu-id="34bef-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34bef-177">The developer of the app.</span></span> <span data-ttu-id="34bef-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-179">notes</span><span class="sxs-lookup"><span data-stu-id="34bef-179">notes</span></span>|<span data-ttu-id="34bef-180">String</span><span class="sxs-lookup"><span data-stu-id="34bef-180">String</span></span>|<span data-ttu-id="34bef-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34bef-181">Notes for the app.</span></span> <span data-ttu-id="34bef-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="34bef-183">uploadState</span></span>|<span data-ttu-id="34bef-184">Int32</span><span class="sxs-lookup"><span data-stu-id="34bef-184">Int32</span></span>|<span data-ttu-id="34bef-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="34bef-185">The upload state.</span></span> <span data-ttu-id="34bef-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="34bef-187">publishingState</span></span>|[<span data-ttu-id="34bef-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="34bef-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="34bef-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34bef-189">The publishing state for the app.</span></span> <span data-ttu-id="34bef-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="34bef-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="34bef-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34bef-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="34bef-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="34bef-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="34bef-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="34bef-193">isAssigned</span></span>|<span data-ttu-id="34bef-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="34bef-194">Boolean</span></span>|<span data-ttu-id="34bef-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="34bef-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="34bef-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34bef-197">roleScopeTagIds</span></span>|<span data-ttu-id="34bef-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="34bef-198">String collection</span></span>|<span data-ttu-id="34bef-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="34bef-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="34bef-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="34bef-201">dependentAppCount</span></span>|<span data-ttu-id="34bef-202">Int32</span><span class="sxs-lookup"><span data-stu-id="34bef-202">Int32</span></span>|<span data-ttu-id="34bef-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="34bef-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="34bef-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34bef-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34bef-205">packageId</span><span class="sxs-lookup"><span data-stu-id="34bef-205">packageId</span></span>|<span data-ttu-id="34bef-206">String</span><span class="sxs-lookup"><span data-stu-id="34bef-206">String</span></span>|<span data-ttu-id="34bef-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="34bef-207">The package identifier.</span></span>|
|<span data-ttu-id="34bef-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="34bef-208">appIdentifier</span></span>|<span data-ttu-id="34bef-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34bef-209">String</span></span>|<span data-ttu-id="34bef-210">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="34bef-210">The Identity Name.</span></span>|
|<span data-ttu-id="34bef-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="34bef-211">usedLicenseCount</span></span>|<span data-ttu-id="34bef-212">Int32</span><span class="sxs-lookup"><span data-stu-id="34bef-212">Int32</span></span>|<span data-ttu-id="34bef-213">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="34bef-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="34bef-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="34bef-214">totalLicenseCount</span></span>|<span data-ttu-id="34bef-215">Int32</span><span class="sxs-lookup"><span data-stu-id="34bef-215">Int32</span></span>|<span data-ttu-id="34bef-216">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="34bef-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="34bef-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="34bef-217">appStoreUrl</span></span>|<span data-ttu-id="34bef-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34bef-218">String</span></span>|<span data-ttu-id="34bef-219">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34bef-219">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="34bef-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="34bef-220">Response</span></span>
<span data-ttu-id="34bef-221">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34bef-221">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34bef-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34bef-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="34bef-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34bef-223">Request</span></span>
<span data-ttu-id="34bef-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34bef-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="34bef-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="34bef-225">Response</span></span>
<span data-ttu-id="34bef-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34bef-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




