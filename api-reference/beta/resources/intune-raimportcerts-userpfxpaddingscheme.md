---
title: Tipo de número userPfxPaddingScheme
description: Valores com suporte para o esquema de preenchimento usado pelo provedor de criptografia.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 64d1ebd0cf28e95264423bf1b5b08bf8d90e7b01
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074819"
---
# <a name="userpfxpaddingscheme-enum-type"></a>Tipo de número userPfxPaddingScheme

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores com suporte para o esquema de preenchimento usado pelo provedor de criptografia.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Esquema de preenchimento desconhecido.|
|pkcs1|1|O Pkcs1 não tem mais suporte|
|oaepSha1|2|OaepSha1 não tem mais suporte|
|oaepSha256|3|Use preenchimento SHA-256 OAEP.|
|oaepSha384|4 |Use preenchimento SHA-384 OAEP.|
|oaepSha512|5 |Use preenchimento SHA-512 OAEP.|



