---
title: Atualizar webApp
description: Atualiza as propriedades de um objeto webApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9528c2fb1818147b09ac1aeb14753e8713006189
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464570"
---
# <a name="update-webapp"></a><span data-ttu-id="26a37-103">Atualizar webApp</span><span class="sxs-lookup"><span data-stu-id="26a37-103">Update webApp</span></span>

<span data-ttu-id="26a37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26a37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26a37-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26a37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26a37-106">Atualiza as propriedades de um objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="26a37-106">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26a37-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26a37-107">Prerequisites</span></span>
<span data-ttu-id="26a37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26a37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26a37-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26a37-110">Permission type</span></span>|<span data-ttu-id="26a37-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26a37-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26a37-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26a37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26a37-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26a37-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="26a37-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26a37-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26a37-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26a37-115">Not supported.</span></span>|
|<span data-ttu-id="26a37-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26a37-116">Application</span></span>|<span data-ttu-id="26a37-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26a37-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26a37-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26a37-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="26a37-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26a37-119">Request headers</span></span>
|<span data-ttu-id="26a37-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26a37-120">Header</span></span>|<span data-ttu-id="26a37-121">Valor</span><span class="sxs-lookup"><span data-stu-id="26a37-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26a37-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26a37-122">Authorization</span></span>|<span data-ttu-id="26a37-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26a37-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26a37-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26a37-124">Accept</span></span>|<span data-ttu-id="26a37-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26a37-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26a37-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26a37-126">Request body</span></span>
<span data-ttu-id="26a37-127">No corpo da solicitação, forneça uma representação JSON do objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="26a37-127">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="26a37-128">A tabela a seguir mostra as propriedades obrigatórias ao criar o [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="26a37-128">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="26a37-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26a37-129">Property</span></span>|<span data-ttu-id="26a37-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="26a37-130">Type</span></span>|<span data-ttu-id="26a37-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="26a37-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26a37-132">id</span><span class="sxs-lookup"><span data-stu-id="26a37-132">id</span></span>|<span data-ttu-id="26a37-133">String</span><span class="sxs-lookup"><span data-stu-id="26a37-133">String</span></span>|<span data-ttu-id="26a37-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="26a37-134">Key of the entity.</span></span> <span data-ttu-id="26a37-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-136">displayName</span><span class="sxs-lookup"><span data-stu-id="26a37-136">displayName</span></span>|<span data-ttu-id="26a37-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26a37-137">String</span></span>|<span data-ttu-id="26a37-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="26a37-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="26a37-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-140">description</span><span class="sxs-lookup"><span data-stu-id="26a37-140">description</span></span>|<span data-ttu-id="26a37-141">String</span><span class="sxs-lookup"><span data-stu-id="26a37-141">String</span></span>|<span data-ttu-id="26a37-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26a37-142">The description of the app.</span></span> <span data-ttu-id="26a37-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-144">publicador</span><span class="sxs-lookup"><span data-stu-id="26a37-144">publisher</span></span>|<span data-ttu-id="26a37-145">String</span><span class="sxs-lookup"><span data-stu-id="26a37-145">String</span></span>|<span data-ttu-id="26a37-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26a37-146">The publisher of the app.</span></span> <span data-ttu-id="26a37-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="26a37-148">largeIcon</span></span>|[<span data-ttu-id="26a37-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="26a37-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="26a37-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="26a37-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="26a37-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26a37-152">createdDateTime</span></span>|<span data-ttu-id="26a37-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26a37-153">DateTimeOffset</span></span>|<span data-ttu-id="26a37-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26a37-154">The date and time the app was created.</span></span> <span data-ttu-id="26a37-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26a37-156">lastModifiedDateTime</span></span>|<span data-ttu-id="26a37-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26a37-157">DateTimeOffset</span></span>|<span data-ttu-id="26a37-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="26a37-158">The date and time the app was last modified.</span></span> <span data-ttu-id="26a37-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="26a37-160">isFeatured</span></span>|<span data-ttu-id="26a37-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="26a37-161">Boolean</span></span>|<span data-ttu-id="26a37-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="26a37-163">privacyInformationUrl</span></span>|<span data-ttu-id="26a37-164">String</span><span class="sxs-lookup"><span data-stu-id="26a37-164">String</span></span>|<span data-ttu-id="26a37-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="26a37-165">The privacy statement Url.</span></span> <span data-ttu-id="26a37-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="26a37-167">informationUrl</span></span>|<span data-ttu-id="26a37-168">String</span><span class="sxs-lookup"><span data-stu-id="26a37-168">String</span></span>|<span data-ttu-id="26a37-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="26a37-169">The more information Url.</span></span> <span data-ttu-id="26a37-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-171">owner</span><span class="sxs-lookup"><span data-stu-id="26a37-171">owner</span></span>|<span data-ttu-id="26a37-172">String</span><span class="sxs-lookup"><span data-stu-id="26a37-172">String</span></span>|<span data-ttu-id="26a37-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="26a37-173">The owner of the app.</span></span> <span data-ttu-id="26a37-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-175">developer</span><span class="sxs-lookup"><span data-stu-id="26a37-175">developer</span></span>|<span data-ttu-id="26a37-176">String</span><span class="sxs-lookup"><span data-stu-id="26a37-176">String</span></span>|<span data-ttu-id="26a37-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26a37-177">The developer of the app.</span></span> <span data-ttu-id="26a37-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-179">notes</span><span class="sxs-lookup"><span data-stu-id="26a37-179">notes</span></span>|<span data-ttu-id="26a37-180">String</span><span class="sxs-lookup"><span data-stu-id="26a37-180">String</span></span>|<span data-ttu-id="26a37-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26a37-181">Notes for the app.</span></span> <span data-ttu-id="26a37-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26a37-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26a37-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="26a37-183">publishingState</span></span>|[<span data-ttu-id="26a37-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="26a37-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="26a37-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26a37-185">The publishing state for the app.</span></span> <span data-ttu-id="26a37-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="26a37-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="26a37-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="26a37-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="26a37-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="26a37-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="26a37-189">appUrl</span><span class="sxs-lookup"><span data-stu-id="26a37-189">appUrl</span></span>|<span data-ttu-id="26a37-190">String</span><span class="sxs-lookup"><span data-stu-id="26a37-190">String</span></span>|<span data-ttu-id="26a37-191">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="26a37-191">The web app URL.</span></span>|
|<span data-ttu-id="26a37-192">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="26a37-192">useManagedBrowser</span></span>|<span data-ttu-id="26a37-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a37-193">Boolean</span></span>|<span data-ttu-id="26a37-194">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="26a37-194">Whether or not to use managed browser.</span></span> <span data-ttu-id="26a37-195">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="26a37-195">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="26a37-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="26a37-196">Response</span></span>
<span data-ttu-id="26a37-197">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [webApp](../resources/intune-apps-webapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26a37-197">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26a37-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26a37-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="26a37-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26a37-199">Request</span></span>
<span data-ttu-id="26a37-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26a37-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26a37-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="26a37-201">Response</span></span>
<span data-ttu-id="26a37-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26a37-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






