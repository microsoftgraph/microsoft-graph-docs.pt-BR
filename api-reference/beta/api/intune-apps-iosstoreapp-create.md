---
title: Criar iosStoreApp
description: Cria um novo objeto iosStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d44dc057415d3095bfc822dc09ba798fcf8ed4ca
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330626"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="dc81e-103">Criar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="dc81e-103">Create iosStoreApp</span></span>

> <span data-ttu-id="dc81e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc81e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc81e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc81e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc81e-106">Cria um novo objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc81e-106">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc81e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc81e-107">Prerequisites</span></span>
<span data-ttu-id="dc81e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc81e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc81e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc81e-110">Permission type</span></span>|<span data-ttu-id="dc81e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc81e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc81e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc81e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc81e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc81e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dc81e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc81e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc81e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc81e-115">Not supported.</span></span>|
|<span data-ttu-id="dc81e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc81e-116">Application</span></span>|<span data-ttu-id="dc81e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc81e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc81e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc81e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="dc81e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc81e-119">Request headers</span></span>
|<span data-ttu-id="dc81e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc81e-120">Header</span></span>|<span data-ttu-id="dc81e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dc81e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc81e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc81e-122">Authorization</span></span>|<span data-ttu-id="dc81e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc81e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc81e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc81e-124">Accept</span></span>|<span data-ttu-id="dc81e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc81e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc81e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc81e-126">Request body</span></span>
<span data-ttu-id="dc81e-127">No corpo da solicitação, forneça uma representação JSON do objeto iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="dc81e-127">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="dc81e-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="dc81e-128">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="dc81e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc81e-129">Property</span></span>|<span data-ttu-id="dc81e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc81e-130">Type</span></span>|<span data-ttu-id="dc81e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc81e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc81e-132">id</span><span class="sxs-lookup"><span data-stu-id="dc81e-132">id</span></span>|<span data-ttu-id="dc81e-133">String</span><span class="sxs-lookup"><span data-stu-id="dc81e-133">String</span></span>|<span data-ttu-id="dc81e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dc81e-134">Key of the entity.</span></span> <span data-ttu-id="dc81e-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dc81e-136">displayName</span></span>|<span data-ttu-id="dc81e-137">String</span><span class="sxs-lookup"><span data-stu-id="dc81e-137">String</span></span>|<span data-ttu-id="dc81e-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="dc81e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dc81e-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-140">descrição</span><span class="sxs-lookup"><span data-stu-id="dc81e-140">description</span></span>|<span data-ttu-id="dc81e-141">String</span><span class="sxs-lookup"><span data-stu-id="dc81e-141">String</span></span>|<span data-ttu-id="dc81e-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc81e-142">The description of the app.</span></span> <span data-ttu-id="dc81e-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-144">publicador</span><span class="sxs-lookup"><span data-stu-id="dc81e-144">publisher</span></span>|<span data-ttu-id="dc81e-145">String</span><span class="sxs-lookup"><span data-stu-id="dc81e-145">String</span></span>|<span data-ttu-id="dc81e-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc81e-146">The publisher of the app.</span></span> <span data-ttu-id="dc81e-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dc81e-148">largeIcon</span></span>|[<span data-ttu-id="dc81e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dc81e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dc81e-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="dc81e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dc81e-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc81e-152">createdDateTime</span></span>|<span data-ttu-id="dc81e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc81e-153">DateTimeOffset</span></span>|<span data-ttu-id="dc81e-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc81e-154">The date and time the app was created.</span></span> <span data-ttu-id="dc81e-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc81e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="dc81e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc81e-157">DateTimeOffset</span></span>|<span data-ttu-id="dc81e-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="dc81e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="dc81e-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dc81e-160">isFeatured</span></span>|<span data-ttu-id="dc81e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc81e-161">Boolean</span></span>|<span data-ttu-id="dc81e-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dc81e-163">privacyInformationUrl</span></span>|<span data-ttu-id="dc81e-164">String</span><span class="sxs-lookup"><span data-stu-id="dc81e-164">String</span></span>|<span data-ttu-id="dc81e-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="dc81e-165">The privacy statement Url.</span></span> <span data-ttu-id="dc81e-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dc81e-167">informationUrl</span></span>|<span data-ttu-id="dc81e-168">String</span><span class="sxs-lookup"><span data-stu-id="dc81e-168">String</span></span>|<span data-ttu-id="dc81e-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="dc81e-169">The more information Url.</span></span> <span data-ttu-id="dc81e-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-171">owner</span><span class="sxs-lookup"><span data-stu-id="dc81e-171">owner</span></span>|<span data-ttu-id="dc81e-172">String</span><span class="sxs-lookup"><span data-stu-id="dc81e-172">String</span></span>|<span data-ttu-id="dc81e-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="dc81e-173">The owner of the app.</span></span> <span data-ttu-id="dc81e-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-175">developer</span><span class="sxs-lookup"><span data-stu-id="dc81e-175">developer</span></span>|<span data-ttu-id="dc81e-176">String</span><span class="sxs-lookup"><span data-stu-id="dc81e-176">String</span></span>|<span data-ttu-id="dc81e-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc81e-177">The developer of the app.</span></span> <span data-ttu-id="dc81e-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-179">notes</span><span class="sxs-lookup"><span data-stu-id="dc81e-179">notes</span></span>|<span data-ttu-id="dc81e-180">String</span><span class="sxs-lookup"><span data-stu-id="dc81e-180">String</span></span>|<span data-ttu-id="dc81e-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc81e-181">Notes for the app.</span></span> <span data-ttu-id="dc81e-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="dc81e-183">uploadState</span></span>|<span data-ttu-id="dc81e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="dc81e-184">Int32</span></span>|<span data-ttu-id="dc81e-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="dc81e-185">The upload state.</span></span> <span data-ttu-id="dc81e-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="dc81e-187">publishingState</span></span>|[<span data-ttu-id="dc81e-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="dc81e-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dc81e-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc81e-189">The publishing state for the app.</span></span> <span data-ttu-id="dc81e-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="dc81e-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dc81e-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc81e-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dc81e-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="dc81e-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dc81e-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="dc81e-193">isAssigned</span></span>|<span data-ttu-id="dc81e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc81e-194">Boolean</span></span>|<span data-ttu-id="dc81e-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="dc81e-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="dc81e-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dc81e-197">roleScopeTagIds</span></span>|<span data-ttu-id="dc81e-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc81e-198">String collection</span></span>|<span data-ttu-id="dc81e-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="dc81e-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="dc81e-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="dc81e-201">dependentAppCount</span></span>|<span data-ttu-id="dc81e-202">Int32</span><span class="sxs-lookup"><span data-stu-id="dc81e-202">Int32</span></span>|<span data-ttu-id="dc81e-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="dc81e-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="dc81e-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc81e-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dc81e-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="dc81e-205">bundleId</span></span>|<span data-ttu-id="dc81e-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc81e-206">String</span></span>|<span data-ttu-id="dc81e-207">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="dc81e-207">The Identity Name.</span></span>|
|<span data-ttu-id="dc81e-208">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="dc81e-208">appStoreUrl</span></span>|<span data-ttu-id="dc81e-209">String</span><span class="sxs-lookup"><span data-stu-id="dc81e-209">String</span></span>|<span data-ttu-id="dc81e-210">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="dc81e-210">The Apple App Store URL</span></span>|
|<span data-ttu-id="dc81e-211">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="dc81e-211">applicableDeviceType</span></span>|[<span data-ttu-id="dc81e-212">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="dc81e-212">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="dc81e-213">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="dc81e-213">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="dc81e-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dc81e-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="dc81e-215">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dc81e-215">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="dc81e-216">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="dc81e-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="dc81e-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc81e-217">Response</span></span>
<span data-ttu-id="dc81e-218">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc81e-218">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc81e-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc81e-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc81e-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc81e-220">Request</span></span>
<span data-ttu-id="dc81e-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc81e-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1140

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
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="dc81e-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc81e-222">Response</span></span>
<span data-ttu-id="dc81e-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc81e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1312

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
    "v12_0": true
  }
}
```






