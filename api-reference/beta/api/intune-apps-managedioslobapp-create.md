---
title: Criar managedIOSLobApp
description: Cria um novo objeto managedIOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 308e9e9c204dd6b81d3b0f90451879a32ca910af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844244"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="cecc2-103">Criar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="cecc2-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="cecc2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cecc2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cecc2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cecc2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cecc2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cecc2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cecc2-107">Cria um novo objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cecc2-107">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cecc2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cecc2-108">Prerequisites</span></span>
<span data-ttu-id="cecc2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cecc2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cecc2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cecc2-111">Permission type</span></span>|<span data-ttu-id="cecc2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cecc2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cecc2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cecc2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cecc2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cecc2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cecc2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cecc2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cecc2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cecc2-116">Not supported.</span></span>|
|<span data-ttu-id="cecc2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cecc2-117">Application</span></span>|<span data-ttu-id="cecc2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cecc2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cecc2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cecc2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cecc2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cecc2-120">Request headers</span></span>
|<span data-ttu-id="cecc2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cecc2-121">Header</span></span>|<span data-ttu-id="cecc2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cecc2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cecc2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cecc2-123">Authorization</span></span>|<span data-ttu-id="cecc2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cecc2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cecc2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cecc2-125">Accept</span></span>|<span data-ttu-id="cecc2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cecc2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cecc2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cecc2-127">Request body</span></span>
<span data-ttu-id="cecc2-128">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="cecc2-128">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="cecc2-129">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="cecc2-129">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="cecc2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cecc2-130">Property</span></span>|<span data-ttu-id="cecc2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cecc2-131">Type</span></span>|<span data-ttu-id="cecc2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cecc2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cecc2-133">id</span><span class="sxs-lookup"><span data-stu-id="cecc2-133">id</span></span>|<span data-ttu-id="cecc2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-134">String</span></span>|<span data-ttu-id="cecc2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cecc2-135">Key of the entity.</span></span> <span data-ttu-id="cecc2-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cecc2-137">displayName</span></span>|<span data-ttu-id="cecc2-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-138">String</span></span>|<span data-ttu-id="cecc2-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="cecc2-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cecc2-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-141">description</span><span class="sxs-lookup"><span data-stu-id="cecc2-141">description</span></span>|<span data-ttu-id="cecc2-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-142">String</span></span>|<span data-ttu-id="cecc2-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cecc2-143">The description of the app.</span></span> <span data-ttu-id="cecc2-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-145">publisher</span><span class="sxs-lookup"><span data-stu-id="cecc2-145">publisher</span></span>|<span data-ttu-id="cecc2-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-146">String</span></span>|<span data-ttu-id="cecc2-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cecc2-147">The publisher of the app.</span></span> <span data-ttu-id="cecc2-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cecc2-149">largeIcon</span></span>|[<span data-ttu-id="cecc2-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cecc2-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cecc2-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="cecc2-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cecc2-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cecc2-153">createdDateTime</span></span>|<span data-ttu-id="cecc2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cecc2-154">DateTimeOffset</span></span>|<span data-ttu-id="cecc2-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cecc2-155">The date and time the app was created.</span></span> <span data-ttu-id="cecc2-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cecc2-157">lastModifiedDateTime</span></span>|<span data-ttu-id="cecc2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cecc2-158">DateTimeOffset</span></span>|<span data-ttu-id="cecc2-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cecc2-159">The date and time the app was last modified.</span></span> <span data-ttu-id="cecc2-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cecc2-161">isFeatured</span></span>|<span data-ttu-id="cecc2-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="cecc2-162">Boolean</span></span>|<span data-ttu-id="cecc2-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cecc2-164">privacyInformationUrl</span></span>|<span data-ttu-id="cecc2-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-165">String</span></span>|<span data-ttu-id="cecc2-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="cecc2-166">The privacy statement Url.</span></span> <span data-ttu-id="cecc2-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cecc2-168">informationUrl</span></span>|<span data-ttu-id="cecc2-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-169">String</span></span>|<span data-ttu-id="cecc2-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="cecc2-170">The more information Url.</span></span> <span data-ttu-id="cecc2-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-172">owner</span><span class="sxs-lookup"><span data-stu-id="cecc2-172">owner</span></span>|<span data-ttu-id="cecc2-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-173">String</span></span>|<span data-ttu-id="cecc2-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cecc2-174">The owner of the app.</span></span> <span data-ttu-id="cecc2-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-176">developer</span><span class="sxs-lookup"><span data-stu-id="cecc2-176">developer</span></span>|<span data-ttu-id="cecc2-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-177">String</span></span>|<span data-ttu-id="cecc2-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cecc2-178">The developer of the app.</span></span> <span data-ttu-id="cecc2-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-180">Observações</span><span class="sxs-lookup"><span data-stu-id="cecc2-180">notes</span></span>|<span data-ttu-id="cecc2-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-181">String</span></span>|<span data-ttu-id="cecc2-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cecc2-182">Notes for the app.</span></span> <span data-ttu-id="cecc2-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="cecc2-184">uploadState</span></span>|<span data-ttu-id="cecc2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="cecc2-185">Int32</span></span>|<span data-ttu-id="cecc2-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="cecc2-186">The upload state.</span></span> <span data-ttu-id="cecc2-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cecc2-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="cecc2-188">publishingState</span></span>|[<span data-ttu-id="cecc2-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cecc2-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cecc2-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cecc2-190">The publishing state for the app.</span></span> <span data-ttu-id="cecc2-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="cecc2-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cecc2-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cecc2-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cecc2-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cecc2-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cecc2-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="cecc2-194">appAvailability</span></span>|[<span data-ttu-id="cecc2-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="cecc2-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="cecc2-196">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cecc2-196">The Application's availability.</span></span> <span data-ttu-id="cecc2-197">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="cecc2-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="cecc2-198">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="cecc2-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="cecc2-199">version</span><span class="sxs-lookup"><span data-stu-id="cecc2-199">version</span></span>|<span data-ttu-id="cecc2-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-200">String</span></span>|<span data-ttu-id="cecc2-201">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cecc2-201">The Application's version.</span></span> <span data-ttu-id="cecc2-202">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="cecc2-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cecc2-203">committedContentVersion</span></span>|<span data-ttu-id="cecc2-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-204">String</span></span>|<span data-ttu-id="cecc2-205">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="cecc2-205">The internal committed content version.</span></span> <span data-ttu-id="cecc2-206">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cecc2-207">fileName</span><span class="sxs-lookup"><span data-stu-id="cecc2-207">fileName</span></span>|<span data-ttu-id="cecc2-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-208">String</span></span>|<span data-ttu-id="cecc2-209">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="cecc2-209">The name of the main Lob application file.</span></span> <span data-ttu-id="cecc2-210">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cecc2-211">size</span><span class="sxs-lookup"><span data-stu-id="cecc2-211">size</span></span>|<span data-ttu-id="cecc2-212">Int64</span><span class="sxs-lookup"><span data-stu-id="cecc2-212">Int64</span></span>|<span data-ttu-id="cecc2-213">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="cecc2-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="cecc2-214">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cecc2-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cecc2-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="cecc2-215">bundleId</span></span>|<span data-ttu-id="cecc2-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-216">String</span></span>|<span data-ttu-id="cecc2-217">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="cecc2-217">The Identity Name.</span></span>|
|<span data-ttu-id="cecc2-218">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="cecc2-218">applicableDeviceType</span></span>|[<span data-ttu-id="cecc2-219">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="cecc2-219">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="cecc2-220">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="cecc2-220">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="cecc2-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cecc2-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cecc2-222">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cecc2-222">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="cecc2-223">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="cecc2-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="cecc2-224">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cecc2-224">expirationDateTime</span></span>|<span data-ttu-id="cecc2-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cecc2-225">DateTimeOffset</span></span>|<span data-ttu-id="cecc2-226">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="cecc2-226">The expiration time.</span></span>|
|<span data-ttu-id="cecc2-227">versionNumber</span><span class="sxs-lookup"><span data-stu-id="cecc2-227">versionNumber</span></span>|<span data-ttu-id="cecc2-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-228">String</span></span>|<span data-ttu-id="cecc2-229">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="cecc2-229">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cecc2-230">buildNumber</span><span class="sxs-lookup"><span data-stu-id="cecc2-230">buildNumber</span></span>|<span data-ttu-id="cecc2-231">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-231">String</span></span>|<span data-ttu-id="cecc2-232">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="cecc2-232">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cecc2-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="cecc2-233">identityVersion</span></span>|<span data-ttu-id="cecc2-234">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecc2-234">String</span></span>|<span data-ttu-id="cecc2-235">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="cecc2-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="cecc2-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="cecc2-236">Response</span></span>
<span data-ttu-id="cecc2-237">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cecc2-237">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cecc2-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cecc2-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="cecc2-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cecc2-239">Request</span></span>
<span data-ttu-id="cecc2-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cecc2-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1421

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="cecc2-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="cecc2-241">Response</span></span>
<span data-ttu-id="cecc2-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cecc2-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1529

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```





