---
title: Criar macOSOfficeSuiteApp
description: Criar um novo objeto macOSOfficeSuiteApp.
ms.openlocfilehash: 4130cd62d8a7744f477a9cc3db773abd06e1b76d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038116"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="ac0fa-103">Criar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="ac0fa-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="ac0fa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac0fa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac0fa-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac0fa-107">Criar um novo objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="ac0fa-107">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac0fa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac0fa-108">Prerequisites</span></span>
<span data-ttu-id="ac0fa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac0fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac0fa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac0fa-111">Permission type</span></span>|<span data-ttu-id="ac0fa-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac0fa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac0fa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac0fa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ac0fa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac0fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-116">Not supported.</span></span>|
|<span data-ttu-id="ac0fa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac0fa-117">Application</span></span>|<span data-ttu-id="ac0fa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac0fa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac0fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ac0fa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac0fa-120">Request headers</span></span>
|<span data-ttu-id="ac0fa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac0fa-121">Header</span></span>|<span data-ttu-id="ac0fa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ac0fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac0fa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac0fa-123">Authorization</span></span>|<span data-ttu-id="ac0fa-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac0fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ac0fa-125">Accept</span></span>|<span data-ttu-id="ac0fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac0fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac0fa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac0fa-127">Request body</span></span>
<span data-ttu-id="ac0fa-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-128">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="ac0fa-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-129">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="ac0fa-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac0fa-130">Property</span></span>|<span data-ttu-id="ac0fa-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac0fa-131">Type</span></span>|<span data-ttu-id="ac0fa-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac0fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac0fa-133">id</span><span class="sxs-lookup"><span data-stu-id="ac0fa-133">id</span></span>|<span data-ttu-id="ac0fa-134">String</span><span class="sxs-lookup"><span data-stu-id="ac0fa-134">String</span></span>|<span data-ttu-id="ac0fa-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-135">Key of the entity.</span></span> <span data-ttu-id="ac0fa-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ac0fa-137">displayName</span></span>|<span data-ttu-id="ac0fa-138">String</span><span class="sxs-lookup"><span data-stu-id="ac0fa-138">String</span></span>|<span data-ttu-id="ac0fa-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ac0fa-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-141">description</span><span class="sxs-lookup"><span data-stu-id="ac0fa-141">description</span></span>|<span data-ttu-id="ac0fa-142">String</span><span class="sxs-lookup"><span data-stu-id="ac0fa-142">String</span></span>|<span data-ttu-id="ac0fa-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-143">The description of the app.</span></span> <span data-ttu-id="ac0fa-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ac0fa-145">publisher</span></span>|<span data-ttu-id="ac0fa-146">String</span><span class="sxs-lookup"><span data-stu-id="ac0fa-146">String</span></span>|<span data-ttu-id="ac0fa-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-147">The publisher of the app.</span></span> <span data-ttu-id="ac0fa-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ac0fa-149">largeIcon</span></span>|[<span data-ttu-id="ac0fa-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ac0fa-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ac0fa-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ac0fa-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac0fa-153">createdDateTime</span></span>|<span data-ttu-id="ac0fa-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac0fa-154">DateTimeOffset</span></span>|<span data-ttu-id="ac0fa-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-155">The date and time the app was created.</span></span> <span data-ttu-id="ac0fa-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac0fa-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ac0fa-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac0fa-158">DateTimeOffset</span></span>|<span data-ttu-id="ac0fa-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ac0fa-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ac0fa-161">isFeatured</span></span>|<span data-ttu-id="ac0fa-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac0fa-162">Boolean</span></span>|<span data-ttu-id="ac0fa-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ac0fa-164">privacyInformationUrl</span></span>|<span data-ttu-id="ac0fa-165">String</span><span class="sxs-lookup"><span data-stu-id="ac0fa-165">String</span></span>|<span data-ttu-id="ac0fa-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-166">The privacy statement Url.</span></span> <span data-ttu-id="ac0fa-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ac0fa-168">informationUrl</span></span>|<span data-ttu-id="ac0fa-169">String</span><span class="sxs-lookup"><span data-stu-id="ac0fa-169">String</span></span>|<span data-ttu-id="ac0fa-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-170">The more information Url.</span></span> <span data-ttu-id="ac0fa-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-172">owner</span><span class="sxs-lookup"><span data-stu-id="ac0fa-172">owner</span></span>|<span data-ttu-id="ac0fa-173">String</span><span class="sxs-lookup"><span data-stu-id="ac0fa-173">String</span></span>|<span data-ttu-id="ac0fa-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-174">The owner of the app.</span></span> <span data-ttu-id="ac0fa-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-176">developer</span><span class="sxs-lookup"><span data-stu-id="ac0fa-176">developer</span></span>|<span data-ttu-id="ac0fa-177">String</span><span class="sxs-lookup"><span data-stu-id="ac0fa-177">String</span></span>|<span data-ttu-id="ac0fa-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-178">The developer of the app.</span></span> <span data-ttu-id="ac0fa-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-180">Observações</span><span class="sxs-lookup"><span data-stu-id="ac0fa-180">notes</span></span>|<span data-ttu-id="ac0fa-181">String</span><span class="sxs-lookup"><span data-stu-id="ac0fa-181">String</span></span>|<span data-ttu-id="ac0fa-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-182">Notes for the app.</span></span> <span data-ttu-id="ac0fa-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ac0fa-184">uploadState</span></span>|<span data-ttu-id="ac0fa-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ac0fa-185">Int32</span></span>|<span data-ttu-id="ac0fa-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-186">The upload state.</span></span> <span data-ttu-id="ac0fa-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac0fa-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac0fa-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ac0fa-188">publishingState</span></span>|[<span data-ttu-id="ac0fa-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ac0fa-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ac0fa-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-190">The publishing state for the app.</span></span> <span data-ttu-id="ac0fa-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ac0fa-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ac0fa-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ac0fa-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="ac0fa-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac0fa-194">Response</span></span>
<span data-ttu-id="ac0fa-195">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-195">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac0fa-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac0fa-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac0fa-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac0fa-197">Request</span></span>
<span data-ttu-id="ac0fa-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 670

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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="ac0fa-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac0fa-199">Response</span></span>
<span data-ttu-id="ac0fa-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac0fa-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 778

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
  "uploadState": 11,
  "publishingState": "processing"
}
```





