AUTOMAKE_OPTIONS = subdir-objects
ACLOCAL_AMFLAGS = ${ACLOCAL_FLAGS}

lib_LTLIBRARIES = libQuantumXML-@QUANTUMXML_API_VERSION@.la

libQuantumXML_@QUANTUMXML_API_VERSION@_la_SOURCES = \
src/Exception.cxx \
src/FSMParser.cxx \
src/Parser.cxx \
src/Stream.cxx \
src/URL.cxx \
src/Validator.cxx \
src/DOM/Attr.cxx \
src/DOM/CDATASection.cxx \
src/DOM/CharacterData.cxx \
src/DOM/Comment.cxx \
src/DOM/Document.cxx \
src/DOM/DocumentFragment.cxx \
src/DOM/DocumentType.cxx \
src/DOM/DOMException.cxx \
src/DOM/DOMImplementation.cxx \
src/DOM/DOMString.cxx \
src/DOM/Element.cxx \
src/DOM/Entity.cxx \
src/DOM/EntityReference.cxx \
src/DOM/NamedNodeMap.cxx \
src/DOM/Node.cxx \
src/DOM/NodeList.cxx \
src/DOM/Notation.cxx \
src/DOM/ProcessingInstruction.cxx \
src/DOM/Text.cxx \
src/fsm/StateBase.cxx \
src/fsm/StateMachine.cxx \
src/states/AttlistDecl.cxx \
src/states/Attribute.cxx \
src/states/CDSect.cxx \
src/states/Comment.cxx \
src/states/DoctypeDecl.cxx \
src/states/Document.cxx \
src/states/Element.cxx \
src/states/ElementDecl.cxx \
src/states/EntityDecl.cxx \
src/states/Misc.cxx \
src/states/NotationDecl.cxx \
src/states/ProcessingInstruction.cxx \
src/states/XMLDecl.cxx \
src/tree/AttDef.cxx \
src/tree/AttList.cxx \
src/tree/Attribute.cxx \
src/tree/CDSect.cxx \
src/tree/CharData.cxx \
src/tree/Comment.cxx \
src/tree/Doctype.cxx \
src/tree/Document.cxx \
src/tree/Element.cxx \
src/tree/ElementDecl.cxx \
src/tree/Entity.cxx \
src/tree/ExternalID.cxx \
src/tree/Misc.cxx \
src/tree/Node.cxx \
src/tree/Notation.cxx \
src/tree/ProcessingInstruction.cxx \
src/tree/Reference.cxx

libQuantumXML_@QUANTUMXML_API_VERSION@_la_LDFLAGS = -version-info $(QUANTUMXML_SO_VERSION)

library_includedir=$(includedir)/QuantumXML-$(QUANTUMXML_API_VERSION)/QuantumXML

library_include_HEADERS= \
src/Exception.h \
src/FSMParser.h \
src/Parser.h \
src/Stream.h \
src/Tree.h \
src/URL.h \
src/Validator.h \
src/XMLString.h \
src/DOM/Attr.h \
src/DOM/CDATASection.h \
src/DOM/CharacterData.h \
src/DOM/Comment.h \
src/DOM/Document.h \
src/DOM/DocumentFragment.h \
src/DOM/DocumentType.h \
src/DOM/DOMException.h \
src/DOM/DOMImplementation.h \
src/DOM/DOMString.h \
src/DOM/Element.h \
src/DOM/Entity.h \
src/DOM/EntityReference.h \
src/DOM/NamedNodeMap.h \
src/DOM/Node.h \
src/DOM/NodeList.h \
src/DOM/Notation.h \
src/DOM/ProcessingInstruction.h \
src/DOM/Text.h \
src/fsm/Functor.h \
src/fsm/MultiState.h \
src/fsm/State.h \
src/fsm/StateBase.h \
src/fsm/StateMachine.h \
src/states/AttlistDecl.h \
src/states/Attribute.h \
src/states/CDSect.h \
src/states/Comment.h \
src/states/DoctypeDecl.h \
src/states/Document.h \
src/states/Element.h \
src/states/ElementDecl.h \
src/states/EntityDecl.h \
src/states/Misc.h \
src/states/NotationDecl.h \
src/states/ProcessingInstruction.h \
src/states/XMLDecl.h \
src/tree/AttDef.h \
src/tree/AttList.h \
src/tree/Attribute.h \
src/tree/CDSect.h \
src/tree/CharData.h \
src/tree/Comment.h \
src/tree/Doctype.h \
src/tree/Document.h \
src/tree/Element.h \
src/tree/ElementDecl.h \
src/tree/Entity.h \
src/tree/ExternalID.h \
src/tree/Misc.h \
src/tree/Node.h \
src/tree/Notation.h \
src/tree/ProcessingInstruction.h \
src/tree/Reference.h


pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = QuantumXML-1.0.pc

dist_noinst_SCRIPTS = autogen.sh
