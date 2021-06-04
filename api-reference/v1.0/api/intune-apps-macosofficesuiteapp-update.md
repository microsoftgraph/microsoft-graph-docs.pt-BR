---
title: Atualizar macOSOfficeSuiteApp
description: Atualizar as propriedades de um objeto  macOSOfficeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 232a4eef3c8543be7d8242c0d8f87586037910fd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754424"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="cd26d-103">Atualizar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="cd26d-103">Update macOSOfficeSuiteApp</span></span>

<span data-ttu-id="cd26d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd26d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd26d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd26d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd26d-106">Atualizar as propriedades de um objeto [ macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd26d-106">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd26d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd26d-107">Prerequisites</span></span>
<span data-ttu-id="cd26d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd26d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd26d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd26d-110">Permission type</span></span>|<span data-ttu-id="cd26d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd26d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd26d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd26d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd26d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd26d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cd26d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd26d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd26d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd26d-115">Not supported.</span></span>|
|<span data-ttu-id="cd26d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd26d-116">Application</span></span>|<span data-ttu-id="cd26d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd26d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd26d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd26d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="cd26d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd26d-119">Request headers</span></span>
|<span data-ttu-id="cd26d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd26d-120">Header</span></span>|<span data-ttu-id="cd26d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cd26d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd26d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd26d-122">Authorization</span></span>|<span data-ttu-id="cd26d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd26d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd26d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd26d-124">Accept</span></span>|<span data-ttu-id="cd26d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd26d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd26d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd26d-126">Request body</span></span>
<span data-ttu-id="cd26d-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd26d-127">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="cd26d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd26d-128">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="cd26d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd26d-129">Property</span></span>|<span data-ttu-id="cd26d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd26d-130">Type</span></span>|<span data-ttu-id="cd26d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd26d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd26d-132">id</span><span class="sxs-lookup"><span data-stu-id="cd26d-132">id</span></span>|<span data-ttu-id="cd26d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd26d-133">String</span></span>|<span data-ttu-id="cd26d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cd26d-134">Key of the entity.</span></span> <span data-ttu-id="cd26d-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cd26d-136">displayName</span></span>|<span data-ttu-id="cd26d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd26d-137">String</span></span>|<span data-ttu-id="cd26d-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="cd26d-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cd26d-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-140">descrição</span><span class="sxs-lookup"><span data-stu-id="cd26d-140">description</span></span>|<span data-ttu-id="cd26d-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd26d-141">String</span></span>|<span data-ttu-id="cd26d-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd26d-142">The description of the app.</span></span> <span data-ttu-id="cd26d-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-144">publicador</span><span class="sxs-lookup"><span data-stu-id="cd26d-144">publisher</span></span>|<span data-ttu-id="cd26d-145">String</span><span class="sxs-lookup"><span data-stu-id="cd26d-145">String</span></span>|<span data-ttu-id="cd26d-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd26d-146">The publisher of the app.</span></span> <span data-ttu-id="cd26d-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cd26d-148">largeIcon</span></span>|[<span data-ttu-id="cd26d-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cd26d-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cd26d-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="cd26d-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cd26d-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd26d-152">createdDateTime</span></span>|<span data-ttu-id="cd26d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd26d-153">DateTimeOffset</span></span>|<span data-ttu-id="cd26d-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd26d-154">The date and time the app was created.</span></span> <span data-ttu-id="cd26d-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd26d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cd26d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd26d-157">DateTimeOffset</span></span>|<span data-ttu-id="cd26d-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cd26d-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cd26d-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cd26d-160">isFeatured</span></span>|<span data-ttu-id="cd26d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd26d-161">Boolean</span></span>|<span data-ttu-id="cd26d-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cd26d-163">privacyInformationUrl</span></span>|<span data-ttu-id="cd26d-164">String</span><span class="sxs-lookup"><span data-stu-id="cd26d-164">String</span></span>|<span data-ttu-id="cd26d-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="cd26d-165">The privacy statement Url.</span></span> <span data-ttu-id="cd26d-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cd26d-167">informationUrl</span></span>|<span data-ttu-id="cd26d-168">String</span><span class="sxs-lookup"><span data-stu-id="cd26d-168">String</span></span>|<span data-ttu-id="cd26d-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="cd26d-169">The more information Url.</span></span> <span data-ttu-id="cd26d-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="cd26d-171">owner</span></span>|<span data-ttu-id="cd26d-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd26d-172">String</span></span>|<span data-ttu-id="cd26d-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cd26d-173">The owner of the app.</span></span> <span data-ttu-id="cd26d-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-175">developer</span><span class="sxs-lookup"><span data-stu-id="cd26d-175">developer</span></span>|<span data-ttu-id="cd26d-176">String</span><span class="sxs-lookup"><span data-stu-id="cd26d-176">String</span></span>|<span data-ttu-id="cd26d-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd26d-177">The developer of the app.</span></span> <span data-ttu-id="cd26d-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-179">notes</span><span class="sxs-lookup"><span data-stu-id="cd26d-179">notes</span></span>|<span data-ttu-id="cd26d-180">String</span><span class="sxs-lookup"><span data-stu-id="cd26d-180">String</span></span>|<span data-ttu-id="cd26d-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd26d-181">Notes for the app.</span></span> <span data-ttu-id="cd26d-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd26d-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd26d-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="cd26d-183">publishingState</span></span>|[<span data-ttu-id="cd26d-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cd26d-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cd26d-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd26d-185">The publishing state for the app.</span></span> <span data-ttu-id="cd26d-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="cd26d-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cd26d-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd26d-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cd26d-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cd26d-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="cd26d-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd26d-189">Response</span></span>
<span data-ttu-id="cd26d-190">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd26d-190">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd26d-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd26d-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd26d-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd26d-192">Request</span></span>
<span data-ttu-id="cd26d-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd26d-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cd26d-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd26d-194">Response</span></span>
<span data-ttu-id="cd26d-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd26d-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




