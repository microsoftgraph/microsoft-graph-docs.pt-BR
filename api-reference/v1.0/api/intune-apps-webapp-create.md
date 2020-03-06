---
title: Criar webApp
description: Cria um novo objeto webApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ee153bac96a29e040b96491c104b9348bc2df09
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515873"
---
# <a name="create-webapp"></a><span data-ttu-id="cb972-103">Criar webApp</span><span class="sxs-lookup"><span data-stu-id="cb972-103">Create webApp</span></span>

<span data-ttu-id="cb972-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb972-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb972-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb972-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb972-106">Cria um novo objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb972-106">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb972-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb972-107">Prerequisites</span></span>
<span data-ttu-id="cb972-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb972-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb972-110">Permission type</span></span>|<span data-ttu-id="cb972-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cb972-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb972-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb972-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb972-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb972-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb972-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb972-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb972-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb972-115">Not supported.</span></span>|
|<span data-ttu-id="cb972-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb972-116">Application</span></span>|<span data-ttu-id="cb972-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb972-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb972-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb972-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cb972-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb972-119">Request headers</span></span>
|<span data-ttu-id="cb972-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb972-120">Header</span></span>|<span data-ttu-id="cb972-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cb972-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb972-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb972-122">Authorization</span></span>|<span data-ttu-id="cb972-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb972-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb972-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb972-124">Accept</span></span>|<span data-ttu-id="cb972-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb972-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb972-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb972-126">Request body</span></span>
<span data-ttu-id="cb972-127">No corpo da solicitação, forneça uma representação JSON do objeto webApp.</span><span class="sxs-lookup"><span data-stu-id="cb972-127">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="cb972-128">A tabela a seguir mostra as propriedades obrigatórias ao criar o webApp.</span><span class="sxs-lookup"><span data-stu-id="cb972-128">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="cb972-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb972-129">Property</span></span>|<span data-ttu-id="cb972-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb972-130">Type</span></span>|<span data-ttu-id="cb972-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb972-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb972-132">id</span><span class="sxs-lookup"><span data-stu-id="cb972-132">id</span></span>|<span data-ttu-id="cb972-133">String</span><span class="sxs-lookup"><span data-stu-id="cb972-133">String</span></span>|<span data-ttu-id="cb972-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cb972-134">Key of the entity.</span></span> <span data-ttu-id="cb972-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cb972-136">displayName</span></span>|<span data-ttu-id="cb972-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb972-137">String</span></span>|<span data-ttu-id="cb972-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="cb972-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cb972-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-140">description</span><span class="sxs-lookup"><span data-stu-id="cb972-140">description</span></span>|<span data-ttu-id="cb972-141">String</span><span class="sxs-lookup"><span data-stu-id="cb972-141">String</span></span>|<span data-ttu-id="cb972-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb972-142">The description of the app.</span></span> <span data-ttu-id="cb972-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-144">publicador</span><span class="sxs-lookup"><span data-stu-id="cb972-144">publisher</span></span>|<span data-ttu-id="cb972-145">String</span><span class="sxs-lookup"><span data-stu-id="cb972-145">String</span></span>|<span data-ttu-id="cb972-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb972-146">The publisher of the app.</span></span> <span data-ttu-id="cb972-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cb972-148">largeIcon</span></span>|[<span data-ttu-id="cb972-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cb972-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cb972-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="cb972-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cb972-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb972-152">createdDateTime</span></span>|<span data-ttu-id="cb972-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb972-153">DateTimeOffset</span></span>|<span data-ttu-id="cb972-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb972-154">The date and time the app was created.</span></span> <span data-ttu-id="cb972-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb972-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cb972-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb972-157">DateTimeOffset</span></span>|<span data-ttu-id="cb972-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cb972-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cb972-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cb972-160">isFeatured</span></span>|<span data-ttu-id="cb972-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="cb972-161">Boolean</span></span>|<span data-ttu-id="cb972-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cb972-163">privacyInformationUrl</span></span>|<span data-ttu-id="cb972-164">String</span><span class="sxs-lookup"><span data-stu-id="cb972-164">String</span></span>|<span data-ttu-id="cb972-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="cb972-165">The privacy statement Url.</span></span> <span data-ttu-id="cb972-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cb972-167">informationUrl</span></span>|<span data-ttu-id="cb972-168">String</span><span class="sxs-lookup"><span data-stu-id="cb972-168">String</span></span>|<span data-ttu-id="cb972-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="cb972-169">The more information Url.</span></span> <span data-ttu-id="cb972-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-171">owner</span><span class="sxs-lookup"><span data-stu-id="cb972-171">owner</span></span>|<span data-ttu-id="cb972-172">String</span><span class="sxs-lookup"><span data-stu-id="cb972-172">String</span></span>|<span data-ttu-id="cb972-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cb972-173">The owner of the app.</span></span> <span data-ttu-id="cb972-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-175">developer</span><span class="sxs-lookup"><span data-stu-id="cb972-175">developer</span></span>|<span data-ttu-id="cb972-176">String</span><span class="sxs-lookup"><span data-stu-id="cb972-176">String</span></span>|<span data-ttu-id="cb972-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb972-177">The developer of the app.</span></span> <span data-ttu-id="cb972-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-179">notes</span><span class="sxs-lookup"><span data-stu-id="cb972-179">notes</span></span>|<span data-ttu-id="cb972-180">String</span><span class="sxs-lookup"><span data-stu-id="cb972-180">String</span></span>|<span data-ttu-id="cb972-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb972-181">Notes for the app.</span></span> <span data-ttu-id="cb972-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb972-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb972-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="cb972-183">publishingState</span></span>|[<span data-ttu-id="cb972-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cb972-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cb972-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb972-185">The publishing state for the app.</span></span> <span data-ttu-id="cb972-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="cb972-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cb972-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb972-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cb972-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cb972-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cb972-189">appUrl</span><span class="sxs-lookup"><span data-stu-id="cb972-189">appUrl</span></span>|<span data-ttu-id="cb972-190">String</span><span class="sxs-lookup"><span data-stu-id="cb972-190">String</span></span>|<span data-ttu-id="cb972-191">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="cb972-191">The web app URL.</span></span>|
|<span data-ttu-id="cb972-192">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="cb972-192">useManagedBrowser</span></span>|<span data-ttu-id="cb972-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb972-193">Boolean</span></span>|<span data-ttu-id="cb972-194">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="cb972-194">Whether or not to use managed browser.</span></span> <span data-ttu-id="cb972-195">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="cb972-195">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="cb972-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb972-196">Response</span></span>
<span data-ttu-id="cb972-197">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb972-197">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb972-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb972-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb972-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb972-199">Request</span></span>
<span data-ttu-id="cb972-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb972-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="cb972-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb972-201">Response</span></span>
<span data-ttu-id="cb972-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb972-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 817

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```




