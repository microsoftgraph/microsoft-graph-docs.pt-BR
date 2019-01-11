---
title: Criar macOSOfficeSuiteApp
description: Criar um novo objeto macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bf65f879832e4687ad3e784d0b09d7234c8920b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840471"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="88ce9-103">Criar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="88ce9-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="88ce9-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="88ce9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88ce9-105">Criar um novo objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="88ce9-105">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88ce9-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88ce9-106">Prerequisites</span></span>
<span data-ttu-id="88ce9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88ce9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88ce9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88ce9-109">Permission type</span></span>|<span data-ttu-id="88ce9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88ce9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88ce9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88ce9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88ce9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88ce9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="88ce9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88ce9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88ce9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88ce9-114">Not supported.</span></span>|
|<span data-ttu-id="88ce9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88ce9-115">Application</span></span>|<span data-ttu-id="88ce9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88ce9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88ce9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88ce9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="88ce9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88ce9-118">Request headers</span></span>
|<span data-ttu-id="88ce9-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88ce9-119">Header</span></span>|<span data-ttu-id="88ce9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="88ce9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88ce9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="88ce9-121">Authorization</span></span>|<span data-ttu-id="88ce9-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88ce9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88ce9-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88ce9-123">Accept</span></span>|<span data-ttu-id="88ce9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="88ce9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88ce9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88ce9-125">Request body</span></span>
<span data-ttu-id="88ce9-126">No corpo da solicitação, forneça uma representação JSON do objeto macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="88ce9-126">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="88ce9-127">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="88ce9-127">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="88ce9-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88ce9-128">Property</span></span>|<span data-ttu-id="88ce9-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="88ce9-129">Type</span></span>|<span data-ttu-id="88ce9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="88ce9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88ce9-131">id</span><span class="sxs-lookup"><span data-stu-id="88ce9-131">id</span></span>|<span data-ttu-id="88ce9-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88ce9-132">String</span></span>|<span data-ttu-id="88ce9-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="88ce9-133">Key of the entity.</span></span> <span data-ttu-id="88ce9-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="88ce9-135">displayName</span></span>|<span data-ttu-id="88ce9-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88ce9-136">String</span></span>|<span data-ttu-id="88ce9-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="88ce9-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="88ce9-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-139">description</span><span class="sxs-lookup"><span data-stu-id="88ce9-139">description</span></span>|<span data-ttu-id="88ce9-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88ce9-140">String</span></span>|<span data-ttu-id="88ce9-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="88ce9-141">The description of the app.</span></span> <span data-ttu-id="88ce9-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-143">publisher</span><span class="sxs-lookup"><span data-stu-id="88ce9-143">publisher</span></span>|<span data-ttu-id="88ce9-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88ce9-144">String</span></span>|<span data-ttu-id="88ce9-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="88ce9-145">The publisher of the app.</span></span> <span data-ttu-id="88ce9-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="88ce9-147">largeIcon</span></span>|[<span data-ttu-id="88ce9-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="88ce9-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="88ce9-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="88ce9-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="88ce9-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88ce9-151">createdDateTime</span></span>|<span data-ttu-id="88ce9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88ce9-152">DateTimeOffset</span></span>|<span data-ttu-id="88ce9-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="88ce9-153">The date and time the app was created.</span></span> <span data-ttu-id="88ce9-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88ce9-155">lastModifiedDateTime</span></span>|<span data-ttu-id="88ce9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88ce9-156">DateTimeOffset</span></span>|<span data-ttu-id="88ce9-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="88ce9-157">The date and time the app was last modified.</span></span> <span data-ttu-id="88ce9-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="88ce9-159">isFeatured</span></span>|<span data-ttu-id="88ce9-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="88ce9-160">Boolean</span></span>|<span data-ttu-id="88ce9-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="88ce9-162">privacyInformationUrl</span></span>|<span data-ttu-id="88ce9-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88ce9-163">String</span></span>|<span data-ttu-id="88ce9-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="88ce9-164">The privacy statement Url.</span></span> <span data-ttu-id="88ce9-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="88ce9-166">informationUrl</span></span>|<span data-ttu-id="88ce9-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88ce9-167">String</span></span>|<span data-ttu-id="88ce9-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="88ce9-168">The more information Url.</span></span> <span data-ttu-id="88ce9-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-170">owner</span><span class="sxs-lookup"><span data-stu-id="88ce9-170">owner</span></span>|<span data-ttu-id="88ce9-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88ce9-171">String</span></span>|<span data-ttu-id="88ce9-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="88ce9-172">The owner of the app.</span></span> <span data-ttu-id="88ce9-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-174">developer</span><span class="sxs-lookup"><span data-stu-id="88ce9-174">developer</span></span>|<span data-ttu-id="88ce9-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88ce9-175">String</span></span>|<span data-ttu-id="88ce9-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="88ce9-176">The developer of the app.</span></span> <span data-ttu-id="88ce9-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-178">Observações</span><span class="sxs-lookup"><span data-stu-id="88ce9-178">notes</span></span>|<span data-ttu-id="88ce9-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88ce9-179">String</span></span>|<span data-ttu-id="88ce9-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="88ce9-180">Notes for the app.</span></span> <span data-ttu-id="88ce9-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="88ce9-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="88ce9-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="88ce9-182">publishingState</span></span>|[<span data-ttu-id="88ce9-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="88ce9-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="88ce9-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="88ce9-184">The publishing state for the app.</span></span> <span data-ttu-id="88ce9-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="88ce9-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="88ce9-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="88ce9-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="88ce9-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="88ce9-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="88ce9-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="88ce9-188">Response</span></span>
<span data-ttu-id="88ce9-189">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88ce9-189">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88ce9-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88ce9-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="88ce9-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88ce9-191">Request</span></span>
<span data-ttu-id="88ce9-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88ce9-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="88ce9-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="88ce9-193">Response</span></span>
<span data-ttu-id="88ce9-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88ce9-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



