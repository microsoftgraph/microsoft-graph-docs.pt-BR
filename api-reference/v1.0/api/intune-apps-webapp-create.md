---
title: Criar webApp
description: Cria um novo objeto webApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 14645ff86b9686ad7f270ecfead143475940bb95
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750333"
---
# <a name="create-webapp"></a><span data-ttu-id="729b8-103">Criar webApp</span><span class="sxs-lookup"><span data-stu-id="729b8-103">Create webApp</span></span>

<span data-ttu-id="729b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="729b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="729b8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="729b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="729b8-106">Cria um novo objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="729b8-106">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="729b8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="729b8-107">Prerequisites</span></span>
<span data-ttu-id="729b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="729b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="729b8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="729b8-110">Permission type</span></span>|<span data-ttu-id="729b8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="729b8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="729b8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="729b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="729b8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="729b8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="729b8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="729b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="729b8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="729b8-115">Not supported.</span></span>|
|<span data-ttu-id="729b8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="729b8-116">Application</span></span>|<span data-ttu-id="729b8-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="729b8-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="729b8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="729b8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="729b8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="729b8-119">Request headers</span></span>
|<span data-ttu-id="729b8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="729b8-120">Header</span></span>|<span data-ttu-id="729b8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="729b8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="729b8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="729b8-122">Authorization</span></span>|<span data-ttu-id="729b8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="729b8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="729b8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="729b8-124">Accept</span></span>|<span data-ttu-id="729b8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="729b8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="729b8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="729b8-126">Request body</span></span>
<span data-ttu-id="729b8-127">No corpo da solicitação, forneça uma representação JSON do objeto webApp.</span><span class="sxs-lookup"><span data-stu-id="729b8-127">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="729b8-128">A tabela a seguir mostra as propriedades obrigatórias ao criar o webApp.</span><span class="sxs-lookup"><span data-stu-id="729b8-128">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="729b8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="729b8-129">Property</span></span>|<span data-ttu-id="729b8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="729b8-130">Type</span></span>|<span data-ttu-id="729b8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="729b8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="729b8-132">id</span><span class="sxs-lookup"><span data-stu-id="729b8-132">id</span></span>|<span data-ttu-id="729b8-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="729b8-133">String</span></span>|<span data-ttu-id="729b8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="729b8-134">Key of the entity.</span></span> <span data-ttu-id="729b8-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="729b8-136">displayName</span></span>|<span data-ttu-id="729b8-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="729b8-137">String</span></span>|<span data-ttu-id="729b8-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="729b8-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="729b8-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-140">descrição</span><span class="sxs-lookup"><span data-stu-id="729b8-140">description</span></span>|<span data-ttu-id="729b8-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="729b8-141">String</span></span>|<span data-ttu-id="729b8-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="729b8-142">The description of the app.</span></span> <span data-ttu-id="729b8-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-144">publicador</span><span class="sxs-lookup"><span data-stu-id="729b8-144">publisher</span></span>|<span data-ttu-id="729b8-145">String</span><span class="sxs-lookup"><span data-stu-id="729b8-145">String</span></span>|<span data-ttu-id="729b8-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="729b8-146">The publisher of the app.</span></span> <span data-ttu-id="729b8-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="729b8-148">largeIcon</span></span>|[<span data-ttu-id="729b8-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="729b8-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="729b8-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="729b8-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="729b8-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="729b8-152">createdDateTime</span></span>|<span data-ttu-id="729b8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="729b8-153">DateTimeOffset</span></span>|<span data-ttu-id="729b8-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="729b8-154">The date and time the app was created.</span></span> <span data-ttu-id="729b8-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="729b8-156">lastModifiedDateTime</span></span>|<span data-ttu-id="729b8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="729b8-157">DateTimeOffset</span></span>|<span data-ttu-id="729b8-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="729b8-158">The date and time the app was last modified.</span></span> <span data-ttu-id="729b8-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="729b8-160">isFeatured</span></span>|<span data-ttu-id="729b8-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="729b8-161">Boolean</span></span>|<span data-ttu-id="729b8-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="729b8-163">privacyInformationUrl</span></span>|<span data-ttu-id="729b8-164">String</span><span class="sxs-lookup"><span data-stu-id="729b8-164">String</span></span>|<span data-ttu-id="729b8-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="729b8-165">The privacy statement Url.</span></span> <span data-ttu-id="729b8-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="729b8-167">informationUrl</span></span>|<span data-ttu-id="729b8-168">String</span><span class="sxs-lookup"><span data-stu-id="729b8-168">String</span></span>|<span data-ttu-id="729b8-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="729b8-169">The more information Url.</span></span> <span data-ttu-id="729b8-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="729b8-171">owner</span></span>|<span data-ttu-id="729b8-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="729b8-172">String</span></span>|<span data-ttu-id="729b8-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="729b8-173">The owner of the app.</span></span> <span data-ttu-id="729b8-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-175">developer</span><span class="sxs-lookup"><span data-stu-id="729b8-175">developer</span></span>|<span data-ttu-id="729b8-176">String</span><span class="sxs-lookup"><span data-stu-id="729b8-176">String</span></span>|<span data-ttu-id="729b8-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="729b8-177">The developer of the app.</span></span> <span data-ttu-id="729b8-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-179">notes</span><span class="sxs-lookup"><span data-stu-id="729b8-179">notes</span></span>|<span data-ttu-id="729b8-180">String</span><span class="sxs-lookup"><span data-stu-id="729b8-180">String</span></span>|<span data-ttu-id="729b8-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="729b8-181">Notes for the app.</span></span> <span data-ttu-id="729b8-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="729b8-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="729b8-183">publishingState</span></span>|[<span data-ttu-id="729b8-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="729b8-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="729b8-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="729b8-185">The publishing state for the app.</span></span> <span data-ttu-id="729b8-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="729b8-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="729b8-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="729b8-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="729b8-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="729b8-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="729b8-189">appUrl</span><span class="sxs-lookup"><span data-stu-id="729b8-189">appUrl</span></span>|<span data-ttu-id="729b8-190">String</span><span class="sxs-lookup"><span data-stu-id="729b8-190">String</span></span>|<span data-ttu-id="729b8-191">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="729b8-191">The web app URL.</span></span> <span data-ttu-id="729b8-192">Essa propriedade não pode ser PATCHed.</span><span class="sxs-lookup"><span data-stu-id="729b8-192">This property cannot be PATCHed.</span></span>|
|<span data-ttu-id="729b8-193">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="729b8-193">useManagedBrowser</span></span>|<span data-ttu-id="729b8-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="729b8-194">Boolean</span></span>|<span data-ttu-id="729b8-195">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="729b8-195">Whether or not to use managed browser.</span></span> <span data-ttu-id="729b8-196">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="729b8-196">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="729b8-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="729b8-197">Response</span></span>
<span data-ttu-id="729b8-198">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="729b8-198">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="729b8-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="729b8-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="729b8-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="729b8-200">Request</span></span>
<span data-ttu-id="729b8-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="729b8-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="729b8-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="729b8-202">Response</span></span>
<span data-ttu-id="729b8-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="729b8-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




