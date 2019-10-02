---
title: Atualizar webApp
description: Atualiza as propriedades de um objeto webApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c34de58546df665a0eb983a18a8d47c7b4613f9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358134"
---
# <a name="update-webapp"></a><span data-ttu-id="25b3c-103">Atualizar webApp</span><span class="sxs-lookup"><span data-stu-id="25b3c-103">Update webApp</span></span>

> <span data-ttu-id="25b3c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25b3c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25b3c-105">Atualiza as propriedades de um objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="25b3c-105">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25b3c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25b3c-106">Prerequisites</span></span>
<span data-ttu-id="25b3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25b3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25b3c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25b3c-109">Permission type</span></span>|<span data-ttu-id="25b3c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25b3c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25b3c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25b3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="25b3c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25b3c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="25b3c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25b3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25b3c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25b3c-114">Not supported.</span></span>|
|<span data-ttu-id="25b3c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25b3c-115">Application</span></span>|<span data-ttu-id="25b3c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25b3c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25b3c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25b3c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="25b3c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25b3c-118">Request headers</span></span>
|<span data-ttu-id="25b3c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25b3c-119">Header</span></span>|<span data-ttu-id="25b3c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="25b3c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25b3c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="25b3c-121">Authorization</span></span>|<span data-ttu-id="25b3c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25b3c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25b3c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25b3c-123">Accept</span></span>|<span data-ttu-id="25b3c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="25b3c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25b3c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25b3c-125">Request body</span></span>
<span data-ttu-id="25b3c-126">No corpo da solicitação, forneça uma representação JSON do objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="25b3c-126">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="25b3c-127">A tabela a seguir mostra as propriedades obrigatórias ao criar o [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="25b3c-127">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="25b3c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25b3c-128">Property</span></span>|<span data-ttu-id="25b3c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="25b3c-129">Type</span></span>|<span data-ttu-id="25b3c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="25b3c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25b3c-131">id</span><span class="sxs-lookup"><span data-stu-id="25b3c-131">id</span></span>|<span data-ttu-id="25b3c-132">String</span><span class="sxs-lookup"><span data-stu-id="25b3c-132">String</span></span>|<span data-ttu-id="25b3c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="25b3c-133">Key of the entity.</span></span> <span data-ttu-id="25b3c-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="25b3c-135">displayName</span></span>|<span data-ttu-id="25b3c-136">String</span><span class="sxs-lookup"><span data-stu-id="25b3c-136">String</span></span>|<span data-ttu-id="25b3c-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="25b3c-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="25b3c-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-139">descrição</span><span class="sxs-lookup"><span data-stu-id="25b3c-139">description</span></span>|<span data-ttu-id="25b3c-140">String</span><span class="sxs-lookup"><span data-stu-id="25b3c-140">String</span></span>|<span data-ttu-id="25b3c-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25b3c-141">The description of the app.</span></span> <span data-ttu-id="25b3c-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-143">publicador</span><span class="sxs-lookup"><span data-stu-id="25b3c-143">publisher</span></span>|<span data-ttu-id="25b3c-144">String</span><span class="sxs-lookup"><span data-stu-id="25b3c-144">String</span></span>|<span data-ttu-id="25b3c-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25b3c-145">The publisher of the app.</span></span> <span data-ttu-id="25b3c-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="25b3c-147">largeIcon</span></span>|[<span data-ttu-id="25b3c-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="25b3c-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="25b3c-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="25b3c-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="25b3c-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25b3c-151">createdDateTime</span></span>|<span data-ttu-id="25b3c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25b3c-152">DateTimeOffset</span></span>|<span data-ttu-id="25b3c-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25b3c-153">The date and time the app was created.</span></span> <span data-ttu-id="25b3c-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25b3c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="25b3c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25b3c-156">DateTimeOffset</span></span>|<span data-ttu-id="25b3c-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="25b3c-157">The date and time the app was last modified.</span></span> <span data-ttu-id="25b3c-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="25b3c-159">isFeatured</span></span>|<span data-ttu-id="25b3c-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="25b3c-160">Boolean</span></span>|<span data-ttu-id="25b3c-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="25b3c-162">privacyInformationUrl</span></span>|<span data-ttu-id="25b3c-163">String</span><span class="sxs-lookup"><span data-stu-id="25b3c-163">String</span></span>|<span data-ttu-id="25b3c-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="25b3c-164">The privacy statement Url.</span></span> <span data-ttu-id="25b3c-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="25b3c-166">informationUrl</span></span>|<span data-ttu-id="25b3c-167">String</span><span class="sxs-lookup"><span data-stu-id="25b3c-167">String</span></span>|<span data-ttu-id="25b3c-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="25b3c-168">The more information Url.</span></span> <span data-ttu-id="25b3c-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-170">owner</span><span class="sxs-lookup"><span data-stu-id="25b3c-170">owner</span></span>|<span data-ttu-id="25b3c-171">String</span><span class="sxs-lookup"><span data-stu-id="25b3c-171">String</span></span>|<span data-ttu-id="25b3c-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="25b3c-172">The owner of the app.</span></span> <span data-ttu-id="25b3c-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-174">developer</span><span class="sxs-lookup"><span data-stu-id="25b3c-174">developer</span></span>|<span data-ttu-id="25b3c-175">String</span><span class="sxs-lookup"><span data-stu-id="25b3c-175">String</span></span>|<span data-ttu-id="25b3c-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25b3c-176">The developer of the app.</span></span> <span data-ttu-id="25b3c-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-178">notes</span><span class="sxs-lookup"><span data-stu-id="25b3c-178">notes</span></span>|<span data-ttu-id="25b3c-179">String</span><span class="sxs-lookup"><span data-stu-id="25b3c-179">String</span></span>|<span data-ttu-id="25b3c-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25b3c-180">Notes for the app.</span></span> <span data-ttu-id="25b3c-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="25b3c-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="25b3c-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="25b3c-182">publishingState</span></span>|[<span data-ttu-id="25b3c-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="25b3c-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="25b3c-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25b3c-184">The publishing state for the app.</span></span> <span data-ttu-id="25b3c-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="25b3c-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="25b3c-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="25b3c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="25b3c-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="25b3c-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="25b3c-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="25b3c-188">appUrl</span></span>|<span data-ttu-id="25b3c-189">String</span><span class="sxs-lookup"><span data-stu-id="25b3c-189">String</span></span>|<span data-ttu-id="25b3c-190">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="25b3c-190">The web app URL.</span></span>|
|<span data-ttu-id="25b3c-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="25b3c-191">useManagedBrowser</span></span>|<span data-ttu-id="25b3c-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="25b3c-192">Boolean</span></span>|<span data-ttu-id="25b3c-193">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="25b3c-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="25b3c-194">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="25b3c-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="25b3c-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="25b3c-195">Response</span></span>
<span data-ttu-id="25b3c-196">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [webApp](../resources/intune-apps-webapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25b3c-196">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25b3c-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25b3c-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="25b3c-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25b3c-198">Request</span></span>
<span data-ttu-id="25b3c-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25b3c-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="25b3c-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="25b3c-200">Response</span></span>
<span data-ttu-id="25b3c-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25b3c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




