---
title: Atualizar macOSOfficeSuiteApp
description: Atualizar as propriedades de um objeto  macOSOfficeSuiteApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: abfbae5b425edc1c3ac04989045ebfe1a65f51d0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516451"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="220e3-103">Atualizar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="220e3-103">Update macOSOfficeSuiteApp</span></span>

<span data-ttu-id="220e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="220e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="220e3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="220e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="220e3-106">Atualizar as propriedades de um objeto [ macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="220e3-106">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="220e3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="220e3-107">Prerequisites</span></span>
<span data-ttu-id="220e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="220e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="220e3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="220e3-110">Permission type</span></span>|<span data-ttu-id="220e3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="220e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="220e3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="220e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="220e3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="220e3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="220e3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="220e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="220e3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="220e3-115">Not supported.</span></span>|
|<span data-ttu-id="220e3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="220e3-116">Application</span></span>|<span data-ttu-id="220e3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="220e3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="220e3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="220e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="220e3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="220e3-119">Request headers</span></span>
|<span data-ttu-id="220e3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="220e3-120">Header</span></span>|<span data-ttu-id="220e3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="220e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="220e3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="220e3-122">Authorization</span></span>|<span data-ttu-id="220e3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="220e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="220e3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="220e3-124">Accept</span></span>|<span data-ttu-id="220e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="220e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="220e3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="220e3-126">Request body</span></span>
<span data-ttu-id="220e3-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="220e3-127">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="220e3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="220e3-128">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="220e3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="220e3-129">Property</span></span>|<span data-ttu-id="220e3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="220e3-130">Type</span></span>|<span data-ttu-id="220e3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="220e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="220e3-132">id</span><span class="sxs-lookup"><span data-stu-id="220e3-132">id</span></span>|<span data-ttu-id="220e3-133">String</span><span class="sxs-lookup"><span data-stu-id="220e3-133">String</span></span>|<span data-ttu-id="220e3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="220e3-134">Key of the entity.</span></span> <span data-ttu-id="220e3-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="220e3-136">displayName</span></span>|<span data-ttu-id="220e3-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="220e3-137">String</span></span>|<span data-ttu-id="220e3-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="220e3-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="220e3-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-140">description</span><span class="sxs-lookup"><span data-stu-id="220e3-140">description</span></span>|<span data-ttu-id="220e3-141">String</span><span class="sxs-lookup"><span data-stu-id="220e3-141">String</span></span>|<span data-ttu-id="220e3-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220e3-142">The description of the app.</span></span> <span data-ttu-id="220e3-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-144">publicador</span><span class="sxs-lookup"><span data-stu-id="220e3-144">publisher</span></span>|<span data-ttu-id="220e3-145">String</span><span class="sxs-lookup"><span data-stu-id="220e3-145">String</span></span>|<span data-ttu-id="220e3-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220e3-146">The publisher of the app.</span></span> <span data-ttu-id="220e3-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="220e3-148">largeIcon</span></span>|[<span data-ttu-id="220e3-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="220e3-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="220e3-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="220e3-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="220e3-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="220e3-152">createdDateTime</span></span>|<span data-ttu-id="220e3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="220e3-153">DateTimeOffset</span></span>|<span data-ttu-id="220e3-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220e3-154">The date and time the app was created.</span></span> <span data-ttu-id="220e3-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="220e3-156">lastModifiedDateTime</span></span>|<span data-ttu-id="220e3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="220e3-157">DateTimeOffset</span></span>|<span data-ttu-id="220e3-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="220e3-158">The date and time the app was last modified.</span></span> <span data-ttu-id="220e3-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="220e3-160">isFeatured</span></span>|<span data-ttu-id="220e3-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="220e3-161">Boolean</span></span>|<span data-ttu-id="220e3-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="220e3-163">privacyInformationUrl</span></span>|<span data-ttu-id="220e3-164">String</span><span class="sxs-lookup"><span data-stu-id="220e3-164">String</span></span>|<span data-ttu-id="220e3-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="220e3-165">The privacy statement Url.</span></span> <span data-ttu-id="220e3-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="220e3-167">informationUrl</span></span>|<span data-ttu-id="220e3-168">String</span><span class="sxs-lookup"><span data-stu-id="220e3-168">String</span></span>|<span data-ttu-id="220e3-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="220e3-169">The more information Url.</span></span> <span data-ttu-id="220e3-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-171">owner</span><span class="sxs-lookup"><span data-stu-id="220e3-171">owner</span></span>|<span data-ttu-id="220e3-172">String</span><span class="sxs-lookup"><span data-stu-id="220e3-172">String</span></span>|<span data-ttu-id="220e3-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="220e3-173">The owner of the app.</span></span> <span data-ttu-id="220e3-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-175">developer</span><span class="sxs-lookup"><span data-stu-id="220e3-175">developer</span></span>|<span data-ttu-id="220e3-176">String</span><span class="sxs-lookup"><span data-stu-id="220e3-176">String</span></span>|<span data-ttu-id="220e3-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220e3-177">The developer of the app.</span></span> <span data-ttu-id="220e3-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-179">notes</span><span class="sxs-lookup"><span data-stu-id="220e3-179">notes</span></span>|<span data-ttu-id="220e3-180">String</span><span class="sxs-lookup"><span data-stu-id="220e3-180">String</span></span>|<span data-ttu-id="220e3-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220e3-181">Notes for the app.</span></span> <span data-ttu-id="220e3-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="220e3-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="220e3-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="220e3-183">publishingState</span></span>|[<span data-ttu-id="220e3-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="220e3-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="220e3-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220e3-185">The publishing state for the app.</span></span> <span data-ttu-id="220e3-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="220e3-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="220e3-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="220e3-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="220e3-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="220e3-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="220e3-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="220e3-189">Response</span></span>
<span data-ttu-id="220e3-190">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="220e3-190">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="220e3-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="220e3-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="220e3-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="220e3-192">Request</span></span>
<span data-ttu-id="220e3-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="220e3-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 584

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="220e3-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="220e3-194">Response</span></span>
<span data-ttu-id="220e3-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="220e3-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "publishingState": "processing"
}
```




