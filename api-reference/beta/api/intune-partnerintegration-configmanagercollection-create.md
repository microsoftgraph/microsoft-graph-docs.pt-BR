---
title: Criar configManagerCollection
description: Crie um novo objeto configManagerCollection.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 945a4bedf5a0680b001307a0d829cebc606c6812
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59070017"
---
# <a name="create-configmanagercollection"></a>Criar configManagerCollection

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configManagerCollections
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto configManagerCollection.

A tabela a seguir mostra as propriedades que são necessárias ao criar o configManagerCollection.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave da Coleção ConfigManager.|
|displayName|Cadeia de caracteres|The DisplayName.|
|collectionIdentifier|Cadeia de Caracteres|O identificador de coleção no SCCM.|
|hierarchyName|String|O HierarchyName.|
|hierarchyIdentifier|Cadeia de Caracteres|O Identificador de Hierarquia.|
|createdDateTime|DateTimeOffset|A data criada.|
|lastModifiedDateTime|DateTimeOffset|A última data modificada.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configManagerCollections
Content-type: application/json
Content-length: 263

{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "displayName": "Display Name value",
  "collectionIdentifier": "Collection Identifier value",
  "hierarchyName": "Hierarchy Name value",
  "hierarchyIdentifier": "Hierarchy Identifier value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 435

{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "id": "5f9d1d76-1d76-5f9d-761d-9d5f761d9d5f",
  "displayName": "Display Name value",
  "collectionIdentifier": "Collection Identifier value",
  "hierarchyName": "Hierarchy Name value",
  "hierarchyIdentifier": "Hierarchy Identifier value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



