---
title: Atualizar webApp
description: Atualiza as propriedades de um objeto webApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e8c40738aaf0e59f384c02df69664dd3a6e320b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580521"
---
# <a name="update-webapp"></a><span data-ttu-id="744c2-103">Atualizar webApp</span><span class="sxs-lookup"><span data-stu-id="744c2-103">Update webApp</span></span>

> <span data-ttu-id="744c2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="744c2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="744c2-105">Atualiza as propriedades de um objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="744c2-105">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="744c2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="744c2-106">Prerequisites</span></span>
<span data-ttu-id="744c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="744c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="744c2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="744c2-109">Permission type</span></span>|<span data-ttu-id="744c2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="744c2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="744c2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="744c2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="744c2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="744c2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="744c2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="744c2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="744c2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="744c2-114">Not supported.</span></span>|
|<span data-ttu-id="744c2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="744c2-115">Application</span></span>|<span data-ttu-id="744c2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="744c2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="744c2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="744c2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="744c2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="744c2-118">Request headers</span></span>
|<span data-ttu-id="744c2-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="744c2-119">Header</span></span>|<span data-ttu-id="744c2-120">Valor</span><span class="sxs-lookup"><span data-stu-id="744c2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="744c2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="744c2-121">Authorization</span></span>|<span data-ttu-id="744c2-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="744c2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="744c2-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="744c2-123">Accept</span></span>|<span data-ttu-id="744c2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="744c2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="744c2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="744c2-125">Request body</span></span>
<span data-ttu-id="744c2-126">No corpo da solicitação, forneça uma representação JSON do objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="744c2-126">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="744c2-127">A tabela a seguir mostra as propriedades obrigatórias ao criar o [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="744c2-127">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="744c2-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="744c2-128">Property</span></span>|<span data-ttu-id="744c2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="744c2-129">Type</span></span>|<span data-ttu-id="744c2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="744c2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="744c2-131">id</span><span class="sxs-lookup"><span data-stu-id="744c2-131">id</span></span>|<span data-ttu-id="744c2-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="744c2-132">String</span></span>|<span data-ttu-id="744c2-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="744c2-133">Key of the entity.</span></span> <span data-ttu-id="744c2-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="744c2-135">displayName</span></span>|<span data-ttu-id="744c2-136">String</span><span class="sxs-lookup"><span data-stu-id="744c2-136">String</span></span>|<span data-ttu-id="744c2-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="744c2-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="744c2-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-139">description</span><span class="sxs-lookup"><span data-stu-id="744c2-139">description</span></span>|<span data-ttu-id="744c2-140">String</span><span class="sxs-lookup"><span data-stu-id="744c2-140">String</span></span>|<span data-ttu-id="744c2-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="744c2-141">The description of the app.</span></span> <span data-ttu-id="744c2-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-143">publicador</span><span class="sxs-lookup"><span data-stu-id="744c2-143">publisher</span></span>|<span data-ttu-id="744c2-144">String</span><span class="sxs-lookup"><span data-stu-id="744c2-144">String</span></span>|<span data-ttu-id="744c2-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="744c2-145">The publisher of the app.</span></span> <span data-ttu-id="744c2-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="744c2-147">largeIcon</span></span>|[<span data-ttu-id="744c2-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="744c2-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="744c2-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="744c2-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="744c2-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="744c2-151">createdDateTime</span></span>|<span data-ttu-id="744c2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="744c2-152">DateTimeOffset</span></span>|<span data-ttu-id="744c2-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="744c2-153">The date and time the app was created.</span></span> <span data-ttu-id="744c2-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="744c2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="744c2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="744c2-156">DateTimeOffset</span></span>|<span data-ttu-id="744c2-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="744c2-157">The date and time the app was last modified.</span></span> <span data-ttu-id="744c2-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="744c2-159">isFeatured</span></span>|<span data-ttu-id="744c2-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="744c2-160">Boolean</span></span>|<span data-ttu-id="744c2-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="744c2-162">privacyInformationUrl</span></span>|<span data-ttu-id="744c2-163">String</span><span class="sxs-lookup"><span data-stu-id="744c2-163">String</span></span>|<span data-ttu-id="744c2-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="744c2-164">The privacy statement Url.</span></span> <span data-ttu-id="744c2-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="744c2-166">informationUrl</span></span>|<span data-ttu-id="744c2-167">String</span><span class="sxs-lookup"><span data-stu-id="744c2-167">String</span></span>|<span data-ttu-id="744c2-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="744c2-168">The more information Url.</span></span> <span data-ttu-id="744c2-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-170">owner</span><span class="sxs-lookup"><span data-stu-id="744c2-170">owner</span></span>|<span data-ttu-id="744c2-171">String</span><span class="sxs-lookup"><span data-stu-id="744c2-171">String</span></span>|<span data-ttu-id="744c2-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="744c2-172">The owner of the app.</span></span> <span data-ttu-id="744c2-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-174">developer</span><span class="sxs-lookup"><span data-stu-id="744c2-174">developer</span></span>|<span data-ttu-id="744c2-175">String</span><span class="sxs-lookup"><span data-stu-id="744c2-175">String</span></span>|<span data-ttu-id="744c2-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="744c2-176">The developer of the app.</span></span> <span data-ttu-id="744c2-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-178">notes</span><span class="sxs-lookup"><span data-stu-id="744c2-178">notes</span></span>|<span data-ttu-id="744c2-179">String</span><span class="sxs-lookup"><span data-stu-id="744c2-179">String</span></span>|<span data-ttu-id="744c2-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="744c2-180">Notes for the app.</span></span> <span data-ttu-id="744c2-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="744c2-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="744c2-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="744c2-182">publishingState</span></span>|[<span data-ttu-id="744c2-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="744c2-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="744c2-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="744c2-184">The publishing state for the app.</span></span> <span data-ttu-id="744c2-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="744c2-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="744c2-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="744c2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="744c2-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="744c2-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="744c2-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="744c2-188">appUrl</span></span>|<span data-ttu-id="744c2-189">String</span><span class="sxs-lookup"><span data-stu-id="744c2-189">String</span></span>|<span data-ttu-id="744c2-190">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="744c2-190">The web app URL.</span></span>|
|<span data-ttu-id="744c2-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="744c2-191">useManagedBrowser</span></span>|<span data-ttu-id="744c2-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="744c2-192">Boolean</span></span>|<span data-ttu-id="744c2-193">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="744c2-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="744c2-194">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="744c2-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="744c2-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="744c2-195">Response</span></span>
<span data-ttu-id="744c2-196">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [webApp](../resources/intune-apps-webapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="744c2-196">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="744c2-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="744c2-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="744c2-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="744c2-198">Request</span></span>
<span data-ttu-id="744c2-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="744c2-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="744c2-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="744c2-200">Response</span></span>
<span data-ttu-id="744c2-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="744c2-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



