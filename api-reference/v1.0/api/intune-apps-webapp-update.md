---
title: Atualizar webApp
description: Atualiza as propriedades de um objeto webApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6bc530da5c29b32d300c8921e5892b27f5dcfcc2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992220"
---
# <a name="update-webapp"></a><span data-ttu-id="0daed-103">Atualizar webApp</span><span class="sxs-lookup"><span data-stu-id="0daed-103">Update webApp</span></span>

<span data-ttu-id="0daed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0daed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0daed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0daed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0daed-106">Atualiza as propriedades de um objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="0daed-106">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0daed-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0daed-107">Prerequisites</span></span>
<span data-ttu-id="0daed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0daed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0daed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0daed-110">Permission type</span></span>|<span data-ttu-id="0daed-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0daed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0daed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0daed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0daed-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0daed-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0daed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0daed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0daed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0daed-115">Not supported.</span></span>|
|<span data-ttu-id="0daed-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0daed-116">Application</span></span>|<span data-ttu-id="0daed-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0daed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0daed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0daed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="0daed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0daed-119">Request headers</span></span>
|<span data-ttu-id="0daed-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0daed-120">Header</span></span>|<span data-ttu-id="0daed-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0daed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0daed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0daed-122">Authorization</span></span>|<span data-ttu-id="0daed-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0daed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0daed-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0daed-124">Accept</span></span>|<span data-ttu-id="0daed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0daed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0daed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0daed-126">Request body</span></span>
<span data-ttu-id="0daed-127">No corpo da solicitação, forneça uma representação JSON do objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="0daed-127">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="0daed-128">A tabela a seguir mostra as propriedades obrigatórias ao criar o [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="0daed-128">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="0daed-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0daed-129">Property</span></span>|<span data-ttu-id="0daed-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0daed-130">Type</span></span>|<span data-ttu-id="0daed-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0daed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0daed-132">id</span><span class="sxs-lookup"><span data-stu-id="0daed-132">id</span></span>|<span data-ttu-id="0daed-133">String</span><span class="sxs-lookup"><span data-stu-id="0daed-133">String</span></span>|<span data-ttu-id="0daed-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0daed-134">Key of the entity.</span></span> <span data-ttu-id="0daed-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0daed-136">displayName</span></span>|<span data-ttu-id="0daed-137">String</span><span class="sxs-lookup"><span data-stu-id="0daed-137">String</span></span>|<span data-ttu-id="0daed-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0daed-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0daed-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-140">description</span><span class="sxs-lookup"><span data-stu-id="0daed-140">description</span></span>|<span data-ttu-id="0daed-141">String</span><span class="sxs-lookup"><span data-stu-id="0daed-141">String</span></span>|<span data-ttu-id="0daed-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0daed-142">The description of the app.</span></span> <span data-ttu-id="0daed-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-144">publicador</span><span class="sxs-lookup"><span data-stu-id="0daed-144">publisher</span></span>|<span data-ttu-id="0daed-145">String</span><span class="sxs-lookup"><span data-stu-id="0daed-145">String</span></span>|<span data-ttu-id="0daed-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0daed-146">The publisher of the app.</span></span> <span data-ttu-id="0daed-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0daed-148">largeIcon</span></span>|[<span data-ttu-id="0daed-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0daed-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0daed-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0daed-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0daed-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0daed-152">createdDateTime</span></span>|<span data-ttu-id="0daed-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0daed-153">DateTimeOffset</span></span>|<span data-ttu-id="0daed-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0daed-154">The date and time the app was created.</span></span> <span data-ttu-id="0daed-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0daed-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0daed-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0daed-157">DateTimeOffset</span></span>|<span data-ttu-id="0daed-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0daed-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0daed-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0daed-160">isFeatured</span></span>|<span data-ttu-id="0daed-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0daed-161">Boolean</span></span>|<span data-ttu-id="0daed-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0daed-163">privacyInformationUrl</span></span>|<span data-ttu-id="0daed-164">String</span><span class="sxs-lookup"><span data-stu-id="0daed-164">String</span></span>|<span data-ttu-id="0daed-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0daed-165">The privacy statement Url.</span></span> <span data-ttu-id="0daed-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0daed-167">informationUrl</span></span>|<span data-ttu-id="0daed-168">String</span><span class="sxs-lookup"><span data-stu-id="0daed-168">String</span></span>|<span data-ttu-id="0daed-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0daed-169">The more information Url.</span></span> <span data-ttu-id="0daed-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="0daed-171">owner</span></span>|<span data-ttu-id="0daed-172">String</span><span class="sxs-lookup"><span data-stu-id="0daed-172">String</span></span>|<span data-ttu-id="0daed-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0daed-173">The owner of the app.</span></span> <span data-ttu-id="0daed-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-175">developer</span><span class="sxs-lookup"><span data-stu-id="0daed-175">developer</span></span>|<span data-ttu-id="0daed-176">String</span><span class="sxs-lookup"><span data-stu-id="0daed-176">String</span></span>|<span data-ttu-id="0daed-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0daed-177">The developer of the app.</span></span> <span data-ttu-id="0daed-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-179">notes</span><span class="sxs-lookup"><span data-stu-id="0daed-179">notes</span></span>|<span data-ttu-id="0daed-180">String</span><span class="sxs-lookup"><span data-stu-id="0daed-180">String</span></span>|<span data-ttu-id="0daed-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0daed-181">Notes for the app.</span></span> <span data-ttu-id="0daed-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0daed-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0daed-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="0daed-183">publishingState</span></span>|[<span data-ttu-id="0daed-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0daed-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0daed-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0daed-185">The publishing state for the app.</span></span> <span data-ttu-id="0daed-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="0daed-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0daed-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0daed-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0daed-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0daed-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0daed-189">appUrl</span><span class="sxs-lookup"><span data-stu-id="0daed-189">appUrl</span></span>|<span data-ttu-id="0daed-190">String</span><span class="sxs-lookup"><span data-stu-id="0daed-190">String</span></span>|<span data-ttu-id="0daed-191">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="0daed-191">The web app URL.</span></span>|
|<span data-ttu-id="0daed-192">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="0daed-192">useManagedBrowser</span></span>|<span data-ttu-id="0daed-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="0daed-193">Boolean</span></span>|<span data-ttu-id="0daed-194">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="0daed-194">Whether or not to use managed browser.</span></span> <span data-ttu-id="0daed-195">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="0daed-195">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="0daed-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="0daed-196">Response</span></span>
<span data-ttu-id="0daed-197">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [webApp](../resources/intune-apps-webapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0daed-197">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0daed-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0daed-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="0daed-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0daed-199">Request</span></span>
<span data-ttu-id="0daed-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0daed-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0daed-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="0daed-201">Response</span></span>
<span data-ttu-id="0daed-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0daed-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









