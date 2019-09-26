---
title: Criar iosStoreApp
description: Cria um novo objeto iosStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8bc40eff34bcc34156d2d5efed0b031903d15f8a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173637"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="0b814-103">Criar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="0b814-103">Create iosStoreApp</span></span>

> <span data-ttu-id="0b814-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b814-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b814-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b814-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b814-106">Cria um novo objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0b814-106">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b814-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b814-107">Prerequisites</span></span>
<span data-ttu-id="0b814-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b814-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b814-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b814-110">Permission type</span></span>|<span data-ttu-id="0b814-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b814-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b814-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b814-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b814-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b814-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b814-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b814-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b814-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b814-115">Not supported.</span></span>|
|<span data-ttu-id="0b814-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b814-116">Application</span></span>|<span data-ttu-id="0b814-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b814-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b814-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b814-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0b814-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b814-119">Request headers</span></span>
|<span data-ttu-id="0b814-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b814-120">Header</span></span>|<span data-ttu-id="0b814-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0b814-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b814-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b814-122">Authorization</span></span>|<span data-ttu-id="0b814-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b814-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b814-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b814-124">Accept</span></span>|<span data-ttu-id="0b814-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b814-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b814-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b814-126">Request body</span></span>
<span data-ttu-id="0b814-127">No corpo da solicitação, forneça uma representação JSON do objeto iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="0b814-127">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="0b814-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="0b814-128">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="0b814-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b814-129">Property</span></span>|<span data-ttu-id="0b814-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b814-130">Type</span></span>|<span data-ttu-id="0b814-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b814-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b814-132">id</span><span class="sxs-lookup"><span data-stu-id="0b814-132">id</span></span>|<span data-ttu-id="0b814-133">String</span><span class="sxs-lookup"><span data-stu-id="0b814-133">String</span></span>|<span data-ttu-id="0b814-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0b814-134">Key of the entity.</span></span> <span data-ttu-id="0b814-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0b814-136">displayName</span></span>|<span data-ttu-id="0b814-137">String</span><span class="sxs-lookup"><span data-stu-id="0b814-137">String</span></span>|<span data-ttu-id="0b814-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0b814-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0b814-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-140">descrição</span><span class="sxs-lookup"><span data-stu-id="0b814-140">description</span></span>|<span data-ttu-id="0b814-141">String</span><span class="sxs-lookup"><span data-stu-id="0b814-141">String</span></span>|<span data-ttu-id="0b814-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0b814-142">The description of the app.</span></span> <span data-ttu-id="0b814-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-144">publicador</span><span class="sxs-lookup"><span data-stu-id="0b814-144">publisher</span></span>|<span data-ttu-id="0b814-145">String</span><span class="sxs-lookup"><span data-stu-id="0b814-145">String</span></span>|<span data-ttu-id="0b814-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0b814-146">The publisher of the app.</span></span> <span data-ttu-id="0b814-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0b814-148">largeIcon</span></span>|[<span data-ttu-id="0b814-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0b814-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0b814-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0b814-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0b814-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b814-152">createdDateTime</span></span>|<span data-ttu-id="0b814-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b814-153">DateTimeOffset</span></span>|<span data-ttu-id="0b814-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0b814-154">The date and time the app was created.</span></span> <span data-ttu-id="0b814-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b814-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0b814-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b814-157">DateTimeOffset</span></span>|<span data-ttu-id="0b814-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0b814-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0b814-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0b814-160">isFeatured</span></span>|<span data-ttu-id="0b814-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b814-161">Boolean</span></span>|<span data-ttu-id="0b814-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0b814-163">privacyInformationUrl</span></span>|<span data-ttu-id="0b814-164">String</span><span class="sxs-lookup"><span data-stu-id="0b814-164">String</span></span>|<span data-ttu-id="0b814-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0b814-165">The privacy statement Url.</span></span> <span data-ttu-id="0b814-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0b814-167">informationUrl</span></span>|<span data-ttu-id="0b814-168">String</span><span class="sxs-lookup"><span data-stu-id="0b814-168">String</span></span>|<span data-ttu-id="0b814-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0b814-169">The more information Url.</span></span> <span data-ttu-id="0b814-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-171">owner</span><span class="sxs-lookup"><span data-stu-id="0b814-171">owner</span></span>|<span data-ttu-id="0b814-172">String</span><span class="sxs-lookup"><span data-stu-id="0b814-172">String</span></span>|<span data-ttu-id="0b814-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0b814-173">The owner of the app.</span></span> <span data-ttu-id="0b814-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-175">developer</span><span class="sxs-lookup"><span data-stu-id="0b814-175">developer</span></span>|<span data-ttu-id="0b814-176">String</span><span class="sxs-lookup"><span data-stu-id="0b814-176">String</span></span>|<span data-ttu-id="0b814-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0b814-177">The developer of the app.</span></span> <span data-ttu-id="0b814-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-179">notes</span><span class="sxs-lookup"><span data-stu-id="0b814-179">notes</span></span>|<span data-ttu-id="0b814-180">String</span><span class="sxs-lookup"><span data-stu-id="0b814-180">String</span></span>|<span data-ttu-id="0b814-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0b814-181">Notes for the app.</span></span> <span data-ttu-id="0b814-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="0b814-183">uploadState</span></span>|<span data-ttu-id="0b814-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0b814-184">Int32</span></span>|<span data-ttu-id="0b814-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="0b814-185">The upload state.</span></span> <span data-ttu-id="0b814-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="0b814-187">publishingState</span></span>|[<span data-ttu-id="0b814-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0b814-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0b814-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0b814-189">The publishing state for the app.</span></span> <span data-ttu-id="0b814-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="0b814-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0b814-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0b814-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="0b814-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0b814-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0b814-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0b814-193">isAssigned</span></span>|<span data-ttu-id="0b814-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b814-194">Boolean</span></span>|<span data-ttu-id="0b814-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="0b814-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0b814-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b814-197">roleScopeTagIds</span></span>|<span data-ttu-id="0b814-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b814-198">String collection</span></span>|<span data-ttu-id="0b814-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="0b814-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0b814-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="0b814-201">dependentAppCount</span></span>|<span data-ttu-id="0b814-202">Int32</span><span class="sxs-lookup"><span data-stu-id="0b814-202">Int32</span></span>|<span data-ttu-id="0b814-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="0b814-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0b814-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0b814-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0b814-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="0b814-205">bundleId</span></span>|<span data-ttu-id="0b814-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b814-206">String</span></span>|<span data-ttu-id="0b814-207">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="0b814-207">The Identity Name.</span></span>|
|<span data-ttu-id="0b814-208">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0b814-208">appStoreUrl</span></span>|<span data-ttu-id="0b814-209">String</span><span class="sxs-lookup"><span data-stu-id="0b814-209">String</span></span>|<span data-ttu-id="0b814-210">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="0b814-210">The Apple App Store URL</span></span>|
|<span data-ttu-id="0b814-211">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="0b814-211">applicableDeviceType</span></span>|[<span data-ttu-id="0b814-212">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="0b814-212">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="0b814-213">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="0b814-213">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="0b814-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0b814-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0b814-215">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0b814-215">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="0b814-216">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="0b814-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="0b814-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b814-217">Response</span></span>
<span data-ttu-id="0b814-218">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b814-218">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b814-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b814-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b814-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b814-220">Request</span></span>
<span data-ttu-id="0b814-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b814-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1160

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="0b814-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b814-222">Response</span></span>
<span data-ttu-id="0b814-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b814-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1332

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  }
}
```




