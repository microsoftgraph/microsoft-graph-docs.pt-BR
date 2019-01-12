---
title: Criar windowsStoreApp
description: Crie um novo objeto de windowsStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ba7809c47cc90054829d5f6ef8ded3f3f58050b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945066"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="4b3be-103">Criar windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="4b3be-103">Create windowsStoreApp</span></span>

> <span data-ttu-id="4b3be-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4b3be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b3be-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4b3be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b3be-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4b3be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b3be-107">Crie um novo objeto de [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="4b3be-107">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b3be-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b3be-108">Prerequisites</span></span>
<span data-ttu-id="4b3be-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b3be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b3be-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b3be-111">Permission type</span></span>|<span data-ttu-id="4b3be-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b3be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b3be-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b3be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b3be-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b3be-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b3be-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b3be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b3be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b3be-116">Not supported.</span></span>|
|<span data-ttu-id="4b3be-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b3be-117">Application</span></span>|<span data-ttu-id="4b3be-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b3be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b3be-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b3be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4b3be-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b3be-120">Request headers</span></span>
|<span data-ttu-id="4b3be-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b3be-121">Header</span></span>|<span data-ttu-id="4b3be-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4b3be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b3be-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b3be-123">Authorization</span></span>|<span data-ttu-id="4b3be-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b3be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b3be-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b3be-125">Accept</span></span>|<span data-ttu-id="4b3be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b3be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b3be-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b3be-127">Request body</span></span>
<span data-ttu-id="4b3be-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsStoreApp.</span><span class="sxs-lookup"><span data-stu-id="4b3be-128">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="4b3be-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsStoreApp.</span><span class="sxs-lookup"><span data-stu-id="4b3be-129">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="4b3be-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b3be-130">Property</span></span>|<span data-ttu-id="4b3be-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b3be-131">Type</span></span>|<span data-ttu-id="4b3be-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b3be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b3be-133">id</span><span class="sxs-lookup"><span data-stu-id="4b3be-133">id</span></span>|<span data-ttu-id="4b3be-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3be-134">String</span></span>|<span data-ttu-id="4b3be-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4b3be-135">Key of the entity.</span></span> <span data-ttu-id="4b3be-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4b3be-137">displayName</span></span>|<span data-ttu-id="4b3be-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3be-138">String</span></span>|<span data-ttu-id="4b3be-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4b3be-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4b3be-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-141">description</span><span class="sxs-lookup"><span data-stu-id="4b3be-141">description</span></span>|<span data-ttu-id="4b3be-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3be-142">String</span></span>|<span data-ttu-id="4b3be-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b3be-143">The description of the app.</span></span> <span data-ttu-id="4b3be-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-145">publisher</span><span class="sxs-lookup"><span data-stu-id="4b3be-145">publisher</span></span>|<span data-ttu-id="4b3be-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3be-146">String</span></span>|<span data-ttu-id="4b3be-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b3be-147">The publisher of the app.</span></span> <span data-ttu-id="4b3be-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4b3be-149">largeIcon</span></span>|[<span data-ttu-id="4b3be-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4b3be-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4b3be-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4b3be-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4b3be-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b3be-153">createdDateTime</span></span>|<span data-ttu-id="4b3be-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b3be-154">DateTimeOffset</span></span>|<span data-ttu-id="4b3be-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b3be-155">The date and time the app was created.</span></span> <span data-ttu-id="4b3be-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b3be-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4b3be-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b3be-158">DateTimeOffset</span></span>|<span data-ttu-id="4b3be-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4b3be-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4b3be-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4b3be-161">isFeatured</span></span>|<span data-ttu-id="4b3be-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="4b3be-162">Boolean</span></span>|<span data-ttu-id="4b3be-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4b3be-164">privacyInformationUrl</span></span>|<span data-ttu-id="4b3be-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3be-165">String</span></span>|<span data-ttu-id="4b3be-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4b3be-166">The privacy statement Url.</span></span> <span data-ttu-id="4b3be-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4b3be-168">informationUrl</span></span>|<span data-ttu-id="4b3be-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3be-169">String</span></span>|<span data-ttu-id="4b3be-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4b3be-170">The more information Url.</span></span> <span data-ttu-id="4b3be-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-172">owner</span><span class="sxs-lookup"><span data-stu-id="4b3be-172">owner</span></span>|<span data-ttu-id="4b3be-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3be-173">String</span></span>|<span data-ttu-id="4b3be-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4b3be-174">The owner of the app.</span></span> <span data-ttu-id="4b3be-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-176">developer</span><span class="sxs-lookup"><span data-stu-id="4b3be-176">developer</span></span>|<span data-ttu-id="4b3be-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3be-177">String</span></span>|<span data-ttu-id="4b3be-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b3be-178">The developer of the app.</span></span> <span data-ttu-id="4b3be-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-180">Observações</span><span class="sxs-lookup"><span data-stu-id="4b3be-180">notes</span></span>|<span data-ttu-id="4b3be-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3be-181">String</span></span>|<span data-ttu-id="4b3be-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b3be-182">Notes for the app.</span></span> <span data-ttu-id="4b3be-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4b3be-184">uploadState</span></span>|<span data-ttu-id="4b3be-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4b3be-185">Int32</span></span>|<span data-ttu-id="4b3be-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="4b3be-186">The upload state.</span></span> <span data-ttu-id="4b3be-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b3be-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b3be-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="4b3be-188">publishingState</span></span>|[<span data-ttu-id="4b3be-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4b3be-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4b3be-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b3be-190">The publishing state for the app.</span></span> <span data-ttu-id="4b3be-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4b3be-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4b3be-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b3be-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4b3be-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4b3be-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4b3be-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4b3be-194">appStoreUrl</span></span>|<span data-ttu-id="4b3be-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3be-195">String</span></span>|<span data-ttu-id="4b3be-196">A URL de repositório de aplicativo do Windows.</span><span class="sxs-lookup"><span data-stu-id="4b3be-196">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="4b3be-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b3be-197">Response</span></span>
<span data-ttu-id="4b3be-198">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b3be-198">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b3be-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b3be-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b3be-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b3be-200">Request</span></span>
<span data-ttu-id="4b3be-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b3be-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 720

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="4b3be-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b3be-202">Response</span></span>
<span data-ttu-id="4b3be-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b3be-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 828

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
  "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





